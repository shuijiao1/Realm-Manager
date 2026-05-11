# realm-manager

水饺自用 Realm 转发管理脚本。

## 一键运行

```bash
bash <(curl -fsSL https://raw.githubusercontent.com/shuijiao1/Realm-Manager/main/realm.sh)
```

## 快捷命令

```bash
bash realm.sh install       # 安装/更新 Realm
bash realm.sh add           # 添加规则
bash realm.sh list          # 查看规则
bash realm.sh delete        # 删除规则
bash realm.sh restart       # 重启服务
bash realm.sh status        # 查看状态
```

## 文件位置

- Realm 安装目录：`/root/realm`
- 配置文件：`/root/realm/config.toml`
- systemd 服务：`realm.service`
- 日志：`/var/log/realm-manager.log`

## 说明

脚本参考常见 Realm 管理脚本的交互思路，重新整理实现：

- 仅支持 `amd64/x86_64` 架构
- 从 `zhboner/realm` GitHub Release 安装最新版
- 支持添加、查看、按 ID 删除转发规则
- 使用 systemd 管理服务
- 支持 cron 每日重启
- 支持脚本本体更新检查
