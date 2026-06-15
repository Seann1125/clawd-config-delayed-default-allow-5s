# Clawd Config Pack: Delayed Default Allow (5s)

[English](README.md) | [简体中文](README.zh-CN.md)

This repository is a standalone config preset for Clawd on Desk.

这是一个独立的 Clawd on Desk 配置预设仓库。

It does three things:

- keeps permission bubbles enabled
- turns on delayed default allow
- auto-approves after 5 seconds if the user does not click

它会做三件事：

- 保持权限气泡开启
- 开启延迟默认同意
- 用户 5 秒内未点击时自动同意

## Important

This repository does not patch, rebuild, or upgrade Clawd on Desk.

这个仓库不会修改、重装或升级 Clawd on Desk 主程序。

It only works on a Clawd build that already supports these preference keys:

- `permissionBubblesEnabled`
- `delayedAutoApprovePermissions`
- `delayedAutoApproveSeconds`

If your Clawd build does not support delayed default allow yet, this package alone will not add the feature.

如果你的 Clawd 构建本身还不支持“延迟默认同意”，这个配置包也不会单独新增该能力。

## Files

- `clawd-prefs.merge.json` - merge these keys into your existing prefs
- `README.md` - English instructions
- `README.zh-CN.md` - Chinese instructions
- `RELEASE_TEMPLATE.md` - reusable English + Chinese release text
- `LICENSE` - repository license

- `clawd-prefs.merge.json`：合并到现有配置中的配置片段
- `README.md`：英文说明
- `README.zh-CN.md`：中文说明
- `RELEASE_TEMPLATE.md`：可复用的中英双语发布文案
- `LICENSE`：仓库许可证

## How Users Install It

1. Back up the current `clawd-prefs.json`.
2. Locate the Clawd user config file:
   - Windows: `%APPDATA%\\clawd-on-desk\\clawd-prefs.json`
   - macOS: `~/Library/Application Support/clawd-on-desk/clawd-prefs.json`
   - Linux: `~/.config/clawd-on-desk/clawd-prefs.json`
3. Open `clawd-prefs.merge.json`.
4. Copy the keys into the existing `clawd-prefs.json`.
5. Save the file.
6. Restart Clawd on Desk.

## 中文使用方式

1. 备份当前的 `clawd-prefs.json`
2. 找到 Clawd 配置文件：
   - Windows：`%APPDATA%\\clawd-on-desk\\clawd-prefs.json`
   - macOS：`~/Library/Application Support/clawd-on-desk/clawd-prefs.json`
   - Linux：`~/.config/clawd-on-desk/clawd-prefs.json`
3. 打开 `clawd-prefs.merge.json`
4. 将其中配置项合并到现有 `clawd-prefs.json`
5. 保存配置
6. 重启 Clawd on Desk

## Included Config

```json
{
  "permissionBubblesEnabled": true,
  "delayedAutoApprovePermissions": true,
  "delayedAutoApproveSeconds": 5
}
```

## License

[MIT](LICENSE)
