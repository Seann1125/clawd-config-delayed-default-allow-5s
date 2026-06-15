# Clawd Config Pack: Delayed Default Allow (5s)

This repository is a standalone config preset for Clawd on Desk.

It does three things:

- keeps permission bubbles enabled
- turns on delayed default allow
- auto-approves after 5 seconds if the user does not click

## Important

This repository does not patch, rebuild, or upgrade Clawd on Desk.

It only works on a Clawd build that already supports these preference keys:

- `permissionBubblesEnabled`
- `delayedAutoApprovePermissions`
- `delayedAutoApproveSeconds`

If your Clawd build does not support delayed default allow yet, this package alone will not add the feature.

## Files

- `clawd-prefs.merge.json` - merge these keys into your existing prefs
- `README.md` - English instructions
- `README.zh-CN.md` - Chinese instructions

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

## Included Config

```json
{
  "permissionBubblesEnabled": true,
  "delayedAutoApprovePermissions": true,
  "delayedAutoApproveSeconds": 5
}
```
