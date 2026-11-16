# Kinhaus firmware

Update site for Kinhaus room nodes. Nodes check `<model>/manifest.json` here every hour and install new releases automatically (switch **Automatic updates** on the node turns this off). Nodes set to **Update channel = Beta** follow `<model>/beta/manifest.json`; a model with no `beta/` folder has no beta build.

Status: prototype firmware for Kinhaus development boards (Phase 0). Not a retail product and not FCC-certified.

| Model | Channel | Version | Notes |
|---|---|---|---|
| ov-1 | stable | 1.2.3 | Update guard for custom builds; battery reads 'no cell' on a floating pin; Self Test passes bare boards |
| ov-2 | stable | 1.4.2 | Update guard for custom builds; battery reads 'no cell' on a floating pin; Self Test passes bare boards |
| ov-1m | stable | 1.2.3 | Update guard for custom builds; battery reads 'no cell' on a floating pin; Self Test passes bare boards |
| ov-2m | stable | 1.4.1 | Encrypted connection: Home Assistant gives each node its own key; radar unit fixes for HA 2027.5 |
| ov-2m | beta | 1.5.0-beta6 | 1.5.0-beta6: beta5 + S2 signed mesh beacons (bench test build) |
| ov-2m-ld2420 | stable | 1.2.2 | Update guard for custom builds; battery reads 'no cell' on a floating pin; Self Test passes bare boards |
| ov-dk1 | stable | 1.2.2 | Update guard for custom builds; battery reads 'no cell' on a floating pin; Self Test passes bare boards |

## Flash a blank board

Open https://web.esphome.io in Chrome or Edge, connect the board over USB-C, choose **Install** and pick `<model>/firmware.factory.bin` from this site. `firmware.ota.bin` is the over-the-air update image; each `manifest.json` lists its MD5.
