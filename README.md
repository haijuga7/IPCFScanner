# IPCFScanner

The main purpose of this tool is to scan CIDR to find IP proxies for CF Vless, but due to program deficiencies, this tool can only be used to scan IPs connected to Cloudflare, so to determine whether the IP is a proxy IP, you have to check again on this website, [click here](https://cfip-check.pages.dev/)
an example is below

![termux](https://raw.githubusercontent.com/haijuga7/IPCFScanner/main/src/Screenshot_20231221-230839_Termux.png) ![chrome](https://raw.githubusercontent.com/haijuga7/IPCFScanner/main/src/Screenshot_20231221-231714_Chrome.png)

## How To Install

```sh
pkg update && pkg upgrade
pkg install git python3
git clone https://github.com/haijuga7/IPCFScanner.git
cd IPCFScanner
python3 -m pip install -r requirements.txt
python3 ipcfscanner.py -h
```

## Usage

for CIDR / IP RANGE
```
python3 ipcfscanner.py -p 10.10.10.0/24
```
for File with format
1.1.1.0/24
2.2.2.0/24
```
python3 ipcfscanner.py -f test_cidr.txt
```
for more information
```
python3 ipcfscanner.py -h
```
