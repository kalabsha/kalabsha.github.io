---
layout: post
title: Git：以 HTTPS 协议克隆项目时免输入账号密码
tags: Git
---

```bash
% cat ~/.gitconfig
[credential]
helper = store --file $HOME/git-credentials/global.gitcredentials    # 指定路径
helper = store    # 默认路径

% cat ~/.git-credentials
https://username:PASSWORD@gitlab.your.domain
```

或者使用 `git config` 命令：

```bash
git config --global credential.helper store    # 如果不存在，此命令会生成 ~/.gitconfig 文件，并向文件中追加一行 `helper = store`
```

参考文档： https://www.cnblogs.com/volnet/p/git-credentials.html

或者用 `git config --global -e`  来编辑


Ubuntu 20.04 系统默认使用 Nano 编辑器，可以用以下命令进行变更：
```bash
# update-alternatives --config editor
There are 4 choices for the alternative editor (providing /usr/bin/editor).

  Selection    Path                Priority   Status
------------------------------------------------------------
* 0            /bin/nano            40        auto mode
  1            /bin/ed             -100       manual mode
  2            /bin/nano            40        manual mode
  3            /usr/bin/vim.basic   30        manual mode
  4            /usr/bin/vim.tiny    15        manual mode

Press <enter> to keep the current choice[*], or type selection number: 3
update-alternatives: using /usr/bin/vim.basic to provide /usr/bin/editor (editor) in manual mode
```

此前可以使用 `select-editor` 命令，但是在 Ubuntu 20.04 未生效
```bash
# select-editor

Select an editor.  To change later, run 'select-editor'.
  1. /bin/nano        <---- easiest
  2. /usr/bin/vim.basic
  3. /usr/bin/vim.tiny
  4. /bin/ed

Choose 1-4 [1]: 2
```
