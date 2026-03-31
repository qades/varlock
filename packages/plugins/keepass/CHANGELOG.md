# @varlock/keepass-plugin

## 0.0.2

### Patch Changes

- [`6ab4fc9`](https://github.com/dmno-dev/varlock/commit/6ab4fc9d7ad0c1eda21e5012be4d08030c35499b) - Add KeePass plugin for loading secrets from KDBX 4.0 databases.

  - `kp()` resolver with `#attribute` syntax, entry name inference from key, and `customAttributesObj` for bulk custom field loading
  - `kpBulk()` resolver for loading all passwords from a group via `@setValuesBulk`
  - `kdbxPassword` data type for master password validation
  - File mode using kdbxweb with pure WASM argon2 (no native addons, works in SEA builds)
  - CLI mode via `keepassxc-cli` with dynamic `useCli` option (e.g., `useCli=forEnv(dev)`)
  - Multiple database instances via `id` param
  - Key file authentication support
  - Add `input` option to `spawnAsync` for streaming stdin to child processes

- Updated dependencies [[`ba61adb`](https://github.com/dmno-dev/varlock/commit/ba61adb19bd5516f0b48827b386fd7170afe66b5), [`6fe325d`](https://github.com/dmno-dev/varlock/commit/6fe325da965c956d1c01c78535c5a5e65524d7a8), [`76c17f8`](https://github.com/dmno-dev/varlock/commit/76c17f8506fb0bd53b5b8d1a87dae25ab517a1ee)]:
  - varlock@0.7.0
