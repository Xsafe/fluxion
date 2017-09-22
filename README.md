# fluxion
wifi。

## Router login page
Share your own router page with a simple script
```
cd scripts
sudo sh router.sh
```

## Installation
```
git clone --recursive https://github.com/FluxionNetwork/fluxion.git # Download the latest revision
cd fluxion # Switch to tool's directory
./fluxion.sh # Run fluxion (missing dependencies will be auto-installed)
```

## :white_check_mark: Included dependency versions
1. Aircrack : 1:1.2-0~rc4-0parrot0
2. Lighttpd : 1.439-1
3. Hostapd  : 1:2.3-2.3 _If you want to compare this type `dpkg -l | grep "name"`_

## :scroll: Changelog
Fluxion gets weekly updates with new features, improvements and bugfixes.
Be sure to check out the [changelog here](https://github.com/FluxionNetwork/fluxion/commits/master).

## :octocat: How to contribute
All contributions are welcome! Code, documentation, graphics or even design suggestions are welcome; use GitHub to its fullest. Submit pull requests, contribute tutorials or other wiki content -- whatever you have to offer, it would be appreciated!

## :book: How it works
* Scan the networks.
* Capture a handshake (can't be used without a valid handshake, it's necessary to verify the password)
* Use WEB Interface *
* Launch a FakeAP instance to imitate the original access point
* Spawns a MDK3 process, which deauthenticates all users connected to the target network, so they can be lured to connect to the FakeAP and enter the WPA password.
* A fake DNS server is launched in order to capture all DNS requests and redirect them to the host running the script
* A captive portal is launched in order to serve a page, which prompts the user to enter their WPA password
* Each submitted password is verified by the handshake captured earlier
* The attack will automatically terminate, as soon as a correct password is submitted


## Note
* Be aware of sites pretending to be related with the Fluxion Project. They may be delivering malware.

* If you are using Microsoft's versions of Ubuntu or the other distros, do not forget to first install a X-server like X-Ming and before running the script run the following `export DISPLAY=:0`





we are Xsafe------We are eager to share ！
