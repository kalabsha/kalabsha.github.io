---
layout: post
title: Kubernetes 入门（一）
tags: Kubernetes, K8s
---

# 1.  初识 Kubernetes
- What
- Why
- How

# 2. 先跑起来
（五到十分钟）示例：kubectl

1. 官网的交互式教程
1. 创建集群 
    `% minikube start`
1. 部署应用
    ```bash
    % kubectl run kubernetes-bootcamp 
    --image=docker.io/jocatalin/kubernetes-bootcamp:v1 
    --port=8080
    ```
1. 访问应用
    ```bash
    % kubectl expose pod/kubernetes-bootcamp 
    --type="NodePort" 
    --port=8080
    ```
1. 扩容、缩容
    ```bash
    % kubectl scale deployments/kubernetes-bootcamp --replicas=3
    % kubectl scale deployments/kubernetes-bootcamp --replicas=2
    ```
1. 滚动更新、版本回退
    ```bash
    % kubectl set image deployments/kubernetes-bootcamp kubernetes-bootcamp=jocatalin/lubernetes-bootcamp:v2
    % kubectl rollout undo deployments/kubernetes-bootcamp
    ```
总结：部署，架构，运行，访问，滚动更新，健康检查

# 3. 基本概念
- Cluster
- Master
- Node
- Pod
- Controller (运行容器) 
- Deployment
- ReplicaSet
- DaemonSet
- StatefulSet
- Job
- Service （访问容器）
- Namespace（资源隔离）……

# 4. 进阶
## 4.1. 数据管理（持久化）
### 4.1.1. Volume
- emptyDir 
    - 对容器而言是持久的
    - 与 Pod 的生命周期一致
- hostPath 
    - 在宿主机真实存在
    - 与 Node 的生命周期一致
- 外部存储（External Storage Provider） 
    - 与 Kubernetes 集群独立
    - 生命周期：永久

### 4.1.2. PV && PVC
- PV: PersistentVolume 管理员
- PVC: PersistentVolumeClaim 普通用户（开发）

## 4.2. Secret & ConfigMap
- 传统的 env 配置、CMDB
- 加密
- 明文配置信息

## 4.3. 包管理器
- Helm: dpkg, apt, rpm, yum, brew, npm, pip, composer, ...
- 架构： 
    - chart（应用信息）-- Helm（客户端）
    - ~~release（运行实例）-- Tiller（服务端）~~

## 4.4. 网络
- 网络模型 
    - Pod 内容器之间的通信
    - Pod 之间的通信
    - Pod 与 Service 之间的通信
    - 外部访问 
    - NodePort
    - LoadBalancer
- 网络方案（CNI：Container Networking Interface 实现） 
    - Flannel
    - Calico
    - Canal
    - Weave Net

## 4.5. Dashboard 看板

## 4.6. 集群监控
- Weave Scope
- Heapster
- Prometheus Operator

## 4.7. 日志管理
- Elasticsearch（搜索引擎、存储、提供查询接口）
- Fluentd（类似 Logstash, Filebeat，采集日志）
- Kibana（Web 展示）

# 接下来做什么？

KubeSphere

---

参考资料：

- [官网](https://kubernetes.io/)
- [CloudMan: 每天 5 分钟玩转 Kubernetes]()
