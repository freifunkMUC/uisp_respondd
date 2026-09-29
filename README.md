# uisp_respondd

> [!IMPORTANT]
> **This project has moved.** uisp_respondd is now the `uisp` backend of [unified_respondd](https://github.com/freifunkMUC/unified_respondd), together with the former unifi_respondd and omada_respondd. This repository is archived and no longer maintained.

## Migrating

1. Install the new package: `pip install 'unified_respondd[uisp]'`
2. Add `backend: uisp` to your config. `controller_url` is the API base URL without `/devices`, e.g. `https://uisp.example.org/nms/api/v2.1`. `controller_port` is no longer used.
3. Point `UNIFIED_RESPONDD_CONFIG_FILE` to your config (or rename it to `unified_respondd.yaml`) and run `unified-respondd`.

Check the output with `unified-respondd --dry-run` before switching. The [migration guide](https://github.com/freifunkMUC/unified_respondd#from-uisp_respondd) lists the behaviour changes.

Respondd for UISP - Airfiber to meshviewer

Demo https://map.ffmuc.net/#!/en/map/68d79aa82d30:

<img width="457" alt="Screenshot 2023-05-04 at 09 01 46" src="https://user-images.githubusercontent.com/6527744/236213586-65245dcb-3161-491a-a5f1-336ec5d9e957.png">

