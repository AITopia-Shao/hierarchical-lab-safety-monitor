# 完整项目内容

这是一个拥有独立 Git 提交历史的完整项目仓库。代码基线为 [AITopia-Shao/lab-safety-monitor](https://github.com/AITopia-Shao/lab-safety-monitor) 的分层升级提交 `b37445fab423b0c0d4e46e8cb4582a66a689544e`，整理日期为 2026-10-22。

| 目录/文件 | 内容 |
| --- | --- |
| `labguard/src/hierarchy/` | 实验楼、实验室、实验台三级协作、联动、记录与恢复 |
| `labguard/src/ui/hierarchy_window.py` | 新版分层监控、拓扑配置、演练与执行结果界面 |
| `labguard/config/hierarchy.json` | 每间实验室的宏观、多个微观、视频源、模型与联动策略 |
| `labguard/models/` | 完整 PPE 与化学器皿模型文件，非占位文件 |
| `labguard/src/core/` | 原安全核心、R1–R9、温度预测、事件与环境控制 |
| `labguard/src/web/`、`labguard/src/ui/` | 原网页、电脑桌面、实验台小屏 |
| `labguard/src/agent/`、`labguard/knowledge/` | 安全助手与实验室安全手册 |
| `labguard/firmware/` | ESP32 固件源码 |
| `labguard/deploy/`、`labguard/tools/`、`labguard/hub/` | 开发板部署、工具与可选画面异常检测 |
| `labguard/tests/` | 原有及分层新增测试 |
| `labguard/macos/`、根目录 `.command` | Mac 独立环境准备、启动与诊断 |
| `docs/`、`slides/` | 设计文档、操作教程、开发记录、截图与既有汇报资料 |

运行环境通过依赖清单安装。缓存、启动日志、个人 API Key、运行数据库与个人报名资料不属于分发内容。已有 PPT 和早期设计资料保留其原始版本，分层功能以最新操作教程为准。

代码基线已通过 150 项测试，以及 desktop、edge、headless 和分层模式的启动检查。本次独立整理保持实现文件一致，只更新首页与本目录说明。

当前分层功能为单机多节点调度，可接入网络视频源；跨主机代理尚未实现。原模型不含火焰、烟雾、加热设备类别，真实识别需要对应权重。实体硬件、Windows/Intel Mac 和规模性能仍待验证。
