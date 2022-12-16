---
layout: post
title: Python Tips
---

这里记录一些 Python 的小贴士。

1. 使用虚拟环境 `pyenv` 和 `pyenv-virtualenv`
    ```bash
    pyenv install 3.10.4 # [TAB] 补全可以列出众多版本以供选择
    pyenv virtualenv 3.10.4 myvenv # 虚拟出一个名为 myvenv 的 3.10.4 版本的 Python 环境
    pyenv shell myvenv # 进入虚拟环境
    ```

1. 使用 PYPI 源的镜像站点
    ```
    pip install -h

    ...
    Package Index Options:
    -i, --index-url <url>       Base URL of the Python Package Index (default https://pypi.tuna.tsinghua.edu.cn/simple). This should point to a
                                repository compliant with PEP 503 (the simple repository API) or a local directory laid out in the same format.
    --extra-index-url <url>     Extra URLs of package indexes to use in addition to --index-url. Should follow the same rules as --index-url.
    --no-index                  Ignore package index (only looking at --find-links URLs instead).
    -f, --find-links <url>      If a URL or path to an html file, then parse for links to archives such as sdist (.tar.gz) or wheel (.whl)
                                files. If a local path or file:// URL that's a directory, then look for archives in the directory listing.
                                Links to VCS project URLs are not supported.
    ...
    ```

    例如：

    ```bash
    pip config set global.index-url https://pypi.douban.com/simple          # 全局
    pip install --upgrade pip --index-url https://pypi.douban.com/simple    # 一次性
    ```

1. Python 内置的 Web 服务器
    ```bash
    python -m http.server 8888  # 在本机 8888 端口开启一个简易的 Web 服务，此为 Python3 版本
    ```
