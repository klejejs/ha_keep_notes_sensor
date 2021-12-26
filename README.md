# Due to other similar Home Assistant integrations being maintained, this repository has been archived.

---

# ha_keep_notes_sensor
Google Keep notes sensor to see your notes in Home Assistant. Use together with [lovelace keep-notes-card](https://github.com/klejejs/lovelace-keep-notes-card) to display your notes in lovelace.

<img src="https://github.com/klejejs/ha_keep_notes_sensor/blob/master/keep_notes_sensor.jpg" alt="Keep Notes Sensor" />

## Installation

Copy `custom_components/keep_notes_sensor` folder to your HA config folder and add sensor to configuration.



To get Google account password, go to [https://myaccount.google.com/apppasswords](https://myaccount.google.com/apppasswords). For `Select app` choose `other` and when you are asked for name, write anything. Then copy your password and use it in `password:` field.

**Keep in mind that you will be able to see your created password only once.**



To get `list_id`, go to [https://keep.google.com/](https://keep.google.com/) and click on a note you wish to use. Then copy the id from the url. See picture below.


<img src="https://github.com/klejejs/ha_keep_notes_sensor/blob/master/keep_url.jpg" alt="Google Keep url" />


**Note:** Although it is advised to use a list as component is created for that, a simple note will work too.

## Example configuration.yaml

```yaml
sensor:
  platform: keep_notes_sensor
  name: "keep_sensor"
  username: "example@example.com"
  password: "emailpassword"
  list_id: "1Ap2XOoT4W4GT8-kSCpvyrDllnwwSFLupBAyjFMcnaZ-PtcW8OwG_rux_2oLPJf878qkm"
```

## Configuration variables

key | type | description
:--- | :--- | :---
**platform (Required)** | string | The platform name.
**name (Required)** | string | Name of the sensor.
**username (Required)** | string | Your gmail email address.
**password (Required)** | string | See installation for password.
**list_id (Required)** | string | See installation for list id.

***
