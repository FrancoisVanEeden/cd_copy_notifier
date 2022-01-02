# cd_copy_notifier
Guess when Rhythmbox process is done copying a CD and notify hosts on the LAN.

## The scenario
Your old laptop running [Mint](https://linuxmint.com/) is connected to your HiFi and you want to copy your CD collection to its hardrive. Mint ships with [Rhythmbox](http://www.rhythmbox.org/) and this will copy the tracks and identify the metadata automatically for you. The only issue is that you have a lot of CD's to work through and Rhythmbox does not notify you when its done copying.

## Getting set up
1. Download this repository to the Mint box.
2. Modify the hostnames in `done_copying_complain` to the IP addresses/hostnames on your LAN.
3. Start `done_copying_complain` on the Mint box.
4. Copy and run `copy_done_listen` on any laptop/PC you want to loudly announce when a CD is done.
5. Install [Termux](https://termux.com/) and [Termux:API](https://wiki.termux.com/wiki/Termux:API) from [F-Droid](https://f-droid.org/) onto your Android phone.
6. Install [nmap](https://nmap.org/) for the `ncat` dependency: in Termux do `pkg install nmap`.
8. Copy `copy_done_notify` into Termux and run the script.
9. Start copying CD's and enjoy the feedme requests coming from the HiFi.
