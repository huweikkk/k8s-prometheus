# 项目名称：k8s 下 Prometheus 监控搭建

## 简介

本项目用于搭建基于 Kubernetes 的 Prometheus 监控体系，包含以下核心组件及版本：

| 组件名称            | 版本号     | Services端口 | Services类型 |
|---------------------|------------|--------------|---------------|
| Kubernetes          | v1.23.6    | -            | -             |
| Prometheus          | v2.32.1    | 30040        | NodePort      |
| Grafana             | v8.3.3     | 30060        | NodePort      |
| kube-state-metrics  | v2.3.0     | 30080        | NodePort      |
| Alertmanager        | v0.27.0    | 30050        | NodePort      |

## 安装说明

- `k8s/` 文件夹包含k8s需监控主组件的 Service 配置文件;
- CoreDNS 默认已内置 Service，不需额外创建；
- kubelet 相关 Service 也无需单独配置。

