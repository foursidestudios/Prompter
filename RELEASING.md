# Releasing an update

1. Make the change in `index.html` and test it on the iPad.
2. Bump the version in **both** places, using the same number:
   - `APP_VERSION = "1.1"` in `index.html`
   - `"version": "1.1"` in `version.json` (update `released` and `notes` too)
3. Commit with a message like `v1.1: what changed`.
4. Push to `main`. GitHub Pages publishes in about a minute.
5. Open Prompter. The sidebar footer should read `Prompter v1.1`.

Anyone with Prompter open sees **Update to v1.1** next to the version number the next time they open the app, or within 6 hours. Tapping it reloads the new version. The button is ignored while the prompter is rolling.

## Version numbers

- `1.0.1` for small fixes
- `1.1` for new features
- `2.0` for big changes

## Rolling back

On GitHub, open the commit history, pick the last good commit and use **Revert**. Bump the version number on the revert so open copies pick it up.
