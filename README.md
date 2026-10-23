# 坚果 TV 云端配置仓库

App 从这里拉两样东西（镜像链：gh-proxy → jsdelivr → raw）：

- **sources.json** — 源地址。站点换域名时改这份文件即可，App 启动时自动拉取，重启生效。
- **update.json + app/*.apk** — 自更新包。用 peach-tv 仓库的 `tools/hub-release.sh` 一键发布。

改完 sources.json 直接 push main 分支即可（jsdelivr 有 ~12h 缓存，急的话去 purge.jsdelivr.net 刷一下）。
