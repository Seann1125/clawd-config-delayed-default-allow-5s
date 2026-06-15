# Release Template

## English

### What this is

This is a standalone config pack for Clawd on Desk.

### What it does

- keeps permission bubbles enabled
- enables delayed default allow
- auto-approves after 5 seconds if the user does not click

### How to use

1. Back up your current `clawd-prefs.json`
2. Open `clawd-prefs.merge.json`
3. Merge the keys into your existing `clawd-prefs.json`
4. Restart Clawd on Desk

### Important

This package does not upgrade Clawd on Desk itself.

It only works on a Clawd build that already supports:

- `permissionBubblesEnabled`
- `delayedAutoApprovePermissions`
- `delayedAutoApproveSeconds`

## 中文

### 这是什么

这是一个独立的 Clawd on Desk 配置包。

### 它会做什么

- 保持权限气泡开启
- 开启延迟默认同意
- 用户 5 秒内未点击时自动同意

### 使用方式

1. 备份你当前的 `clawd-prefs.json`
2. 打开 `clawd-prefs.merge.json`
3. 将其中配置项合并到现有 `clawd-prefs.json`
4. 重启 Clawd on Desk

### 重要说明

这个包不会升级 Clawd on Desk 主程序。

它只适用于已经支持以下配置项的 Clawd 构建：

- `permissionBubblesEnabled`
- `delayedAutoApprovePermissions`
- `delayedAutoApproveSeconds`
