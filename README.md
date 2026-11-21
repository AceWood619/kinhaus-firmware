# Kinhaus firmware

Update site for Kinhaus room nodes. Nodes check `<model>/manifest.json` here every hour and install new releases automatically (switch **Automatic updates** on the node turns this off). Nodes set to **Update channel = Beta** follow `<model>/beta/manifest.json`; a model with no `beta/` folder has no beta build.

Status: prototype firmware for Kinhaus development boards (Phase 0). Not a retail product and not FCC-certified.

Release notes here stay short on purpose ("Fixes and improvements"). Detailed change notes are kept privately.

| Model | Channel | Version | Notes |
|---|---|---|---|
| ov-1 | stable | 1.2.3 | Fixes and improvements |
| ov-2 | stable | 1.4.2 | Fixes and improvements |
| ov-1m | stable | 1.2.3 | Fixes and improvements |
| ov-2m | stable | 1.4.1 | Fixes and improvements |
| ov-2m | beta | 1.5.0-beta6 | Fixes and improvements |
| ov-2m-ld2420 | stable | 1.2.2 | Fixes and improvements |
| ov-dk1 | stable | 1.2.2 | Fixes and improvements |

## Flash a blank board

Open https://web.esphome.io in Chrome or Edge, connect the board over USB-C, choose **Install** and pick `<model>/firmware.factory.bin` from this site. `firmware.ota.bin` is the over-the-air update image; each `manifest.json` lists its MD5.
