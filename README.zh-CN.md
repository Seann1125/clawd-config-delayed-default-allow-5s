# Clawd 配置包：5 秒延迟默认同意

[English](README.md) | [简体中文](README.zh-CN.md)

这是一个独立的 Clawd on Desk 配置发布包，不是程序安装包，也不是程序升级包。

它会开启以下行为：

- 保持权限气泡开启
- 开启延迟默认同意
- 当用户在 5 秒内没有点击确认时，由 Clawd 自动执行默认同意

## 重要说明

这个包不会修改、重装或升级 Clawd on Desk 主程序。

它只是给 `clawd-prefs.json` 提供一组可合并的基础配置。

它只适用于已经内置以下配置项支持的 Clawd 版本或自定义构建：

- `permissionBubblesEnabled`
- `delayedAutoApprovePermissions`
- `delayedAutoApproveSeconds`

如果用户当前使用的 Clawd 程序本身还不支持“延迟默认同意”，那么只安装这个配置包不会凭空新增这个能力。

## 仓库文件

- `clawd-prefs.merge.json`：配置片段
- `README.md`：英文说明
- `README.zh-CN.md`：中文说明
- `RELEASE_TEMPLATE.md`：可复用的中英双语发布文案
- `LICENSE`：仓库许可证

## 下载用户怎么使用

1. 先备份自己的 `clawd-prefs.json`
2. 找到 Clawd 配置文件位置
   - Windows：`%APPDATA%\\clawd-on-desk\\clawd-prefs.json`
   - macOS：`~/Library/Application Support/clawd-on-desk/clawd-prefs.json`
   - Linux：`~/.config/clawd-on-desk/clawd-prefs.json`
3. 打开本仓库里的 `clawd-prefs.merge.json`
4. 将里面的 3 个配置项合并到自己现有的 `clawd-prefs.json` 中
5. 保存后重启 Clawd on Desk

不要直接用这个 JSON 覆盖整个 `clawd-prefs.json`，否则用户原有的其他设置可能会丢失。

## 本仓库提供的配置

```json
{
  "permissionBubblesEnabled": true,
  "delayedAutoApprovePermissions": true,
  "delayedAutoApproveSeconds": 5
}
```

## 许可证

[MIT](LICENSE)
