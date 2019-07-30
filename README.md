# ha_keep_notes_sensor
Google Keep notes sensor to see your notes in Home Assistant

<img src="https://github.com/klejejs/ha_keep_notes_sensor/blob/master/keep_notes_sensor.jpg" alt="Keep Notes Card" />

## Installation

## Example configuration.yaml

```yaml
sensor:
  platform: keep_notes_sensor
  username: "example@example.com"
  password: "emailpassword"
  list_id: "1Ap2XOoT4W4GT8-kSCpvyrDllnwwSFLupBAyjFMcnaZ-PtcW8OwG_rux_2oLPJf878qkm"
```

## Configuration variables

key | type | description
:--- | :--- | :---
**platform (Required)** | string | The platform name.
**username (Required)** | string | Your gmail email address.
**username (Required)** | string | See installation for password.
**username (Required)** | string | See installation for list id.

***
