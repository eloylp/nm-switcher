# nm-switcher
A helper for switching to the best available wifi network on Linux (network manager)


## Behaviours

* The switcher will only take action when there's at least one active wifi.
* The switcher will select the best known network to connect to, based on the signal strength.

## Commands used by the switcher

* Get current active wifi
```bash
nmcli connection show --active
```
* Get available wifis

```bash
nmcli device wifi list
```
* Get known wifis
```bash
nmcli connection show
```
* Connect to specific wifi
```bash
nmcli device wifi connect <SSID_or_BSSID>
```
