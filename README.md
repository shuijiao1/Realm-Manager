# Realm-Manager

![Shell](https://img.shields.io/badge/Shell-Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)
![Version](https://img.shields.io/badge/version-v0.1.5-blue?style=flat-square)

**中文** | [English](README.en.md)

**Realm 转发管理脚本。**

> 面向 Debian / Ubuntu root 环境，优先使用自己的短链一键运行。

---

## 🎯 核心特性

- 安装 / 更新 Realm 核心
- 添加、查看、删除转发规则
- systemd 服务管理
- 支持 cron 每日重启

---

## 🚀 快速开始

```bash
bash <(curl -Ls https://realm.shuijiao.de)
```

---

---

## ⚠️ 注意事项

- 请在可信 VPS 上以 root 执行。
- 涉及防火墙、SSH、重装、转发规则等操作前，建议保留一个现有 SSH 会话不断开。
