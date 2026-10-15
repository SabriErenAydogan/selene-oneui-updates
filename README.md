# selene-oneui-updates

Update index and delta packages for the One UI port on selene (Redmi 10 2022).

- `versions.txt`: version list. `flash_all.bat` / `flash_all_except_data_storage.bat`
  in the ROM package compare the MD5 of `images\super.img` with it.
  If a newer version exists, the delta packages are downloaded from this
  repo's releases and applied with xdelta before flashing.
- Releases: one per version, tagged with the version (for example `20261101`).
  Each holds `OneUI-selene-update-<from>-to-<to>.zip`.

Skip the update check with `set SABRINIUM_NO_UPDATE=1` before running the flash script.
