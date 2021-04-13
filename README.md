# lwipwin32
lwipwin32 VC++ 2015  

ip
```
  IP4_ADDR(&ip, 192, 168, 137, 121); // lwip ip address
  IP4_ADDR(&mask, 255, 255, 0, 0);   // mask
  IP4_ADDR(&gw, 192, 168, 137, 2);   // VMware Virtual Ethernet Adapter for VMnet8 ip address
```

# run

use VMware Virtual Ethernet Adapter for VMnet8

```
1. \Device\NPF_{0A0C7D05-BE74-46F0-A69E-8984DADF32ED} (Microsoft)
2. \Device\NPF_{8FD0F8EC-D5AA-4FA8-BED6-6E7671C6BBCE} (VMware Virtual Ethernet Adapter)
3. \Device\NPF_{EBC278C8-BF54-4A04-94B8-C382335EE3BA} (VMware Virtual Ethernet Adapter)
4. \Device\NPF_{0589DF01-9E1D-47C1-9FE6-FBF863653E12} (Microsoft)
5. \Device\NPF_{3360C3DC-F23A-4BE0-982E-B21B8B0C83E2} (Microsoft)
6. \Device\NPF_{5515DB08-0F26-41F5-AA3C-3B4747B687AD} (Intel(R) Ethernet Connection (5) I219-LM)
Enter the interface number (1-6):3

listening on VMware Virtual Ethernet Adapter...
```

ping
```
Microsoft Windows [Version 10.0.18362.30]
(c) 2019 Microsoft Corporation. All rights reserved.

C:\Users\bluesky>ping 192.168.137.121

Pinging 192.168.137.121 with 32 bytes of data:
Reply from 192.168.137.121: bytes=32 time=2ms TTL=255
Reply from 192.168.137.121: bytes=32 time=1ms TTL=255
Reply from 192.168.137.121: bytes=32 time=1ms TTL=255
Reply from 192.168.137.121: bytes=32 time=2ms TTL=255

Ping statistics for 192.168.137.121:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 1ms, Maximum = 2ms, Average = 1ms
```
