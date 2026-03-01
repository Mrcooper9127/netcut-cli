## Features:

- scan network
- cut network
- bandwidth limiting (in dev)

scan network
```bash
sudo go run ./main.go -scan -cidr 192.168.0.0/24 -i wlp49s0
```

to cut off a device
```bash
sudo go run ./main.go -i wlp49s0 -cut -ip 192.168.1.142
```
output
```
Scanning network 192.168.0.2/32...
Waiting for responses...
Discovered device: IP=192.168.1.142 MAC=22:0c:a6:f6:38:76 HOSTNAME:[Witchuda-Shop-2.4G]
Stopping packet capture after scan completion.
2026/03/02 00:00:25 Cut off device: IP:192.168.1.142 MAC: HOSTNAME: [Witchuda-Shop-2.4G]
```