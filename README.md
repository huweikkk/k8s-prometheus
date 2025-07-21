# 项目名称：k8s 下 Prometheus 监控搭建

## 简介

本项目用于搭建基于 Kubernetes 的 Prometheus 监控体系，包含以下核心组件及版本：

| 组件名称            | 版本号     |
|---------------------|------------|
| Kubernetes          | v1.23.6    |
| Prometheus          | v2.32.1    |
| Grafana             | v8.3.3     |
| kube-state-metrics  | v2.3.0     |
| Alertmanager        | v0.27.0    |

## 安装说明

- `k8s/` 文件夹包含各个组件的 Service 配置文件（如 Prometheus、Grafana 等）；
- CoreDNS 默认已内置 Service，不需额外创建；
- kubelet 相关 Service 也无需单独配置。
