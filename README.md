# 4.Execution_of_NetworkCommands
## AIM :Use of Network commands in Real Time environment
## Software : Command Prompt And Network Protocol Analyzer
## Procedure: To do this EXPERIMENT- follows these steps:
<BR>
In this EXPERIMENT- students have to understand basic networking commands e.g cpdump, netstat, ifconfig, nslookup ,traceroute and also Capture ping and traceroute PDUs using a network protocol analyzer 
<BR>
All commands related to Network configuration which includes how to switch to privilege mode
<BR>
and normal mode and how to configure router interface and how to save this configuration to
<BR>
flash memory or permanent memory.
<BR>
This commands includes
<BR>
• Configuring the Router commands
<BR>
• General Commands to configure network
<BR>
• Privileged Mode commands of a router 
<BR>
• Router Processes & Statistics
<BR>
• IP Commands
<BR>
• Other IP Commands e.g. show ip route etc.
<BR>

## Output
Microsoft Windows [Version 10.0.26200.8246]
(c) Microsoft Corporation. All rights reserved.

## 1. ping
```
## C:\Users\acer>ping google.com

Pinging google.com [2404:6800:4007:836::200e] with 32 bytes of data:
Reply from 2404:6800:4007:836::200e: time=8ms
Reply from 2404:6800:4007:836::200e: time=14ms
Reply from 2404:6800:4007:836::200e: time=22ms
Reply from 2404:6800:4007:836::200e: time=22ms

Ping statistics for 2404:6800:4007:836::200e:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 8ms, Maximum = 22ms, Average = 16ms
```
## 2.ipconfig
```
## C:\Users\acer>ipconfig

Windows IP Configuration


Wireless LAN adapter Local Area Connection* 1:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Local Area Connection* 2:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :

Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . : saveetha.in
   IPv6 Address. . . . . . . . . . . : 2403:8600:c090:42:0:401:9bfa:fd9f
   Link-local IPv6 Address . . . . . : fe80::d30d:62b0:7886:c7b9%18
   Autoconfiguration IPv4 Address. . : 169.254.235.4
   Subnet Mask . . . . . . . . . . . : 255.255.0.0
   Default Gateway . . . . . . . . . : fe80::eedd:24ff:fe3d:ced5%18

Ethernet adapter Ethernet:

   Media State . . . . . . . . . . . : Media disconnected
   Connection-specific DNS Suffix  . :
```
## 3.tracert
```
## C:\Users\acer>tracert google.com

Tracing route to google.com [2404:6800:4007:836::200e]
over a maximum of 30 hops:

  1    86 ms     6 ms     8 ms  2403:8600:c090:42::1
  2     *        *        *     Request timed out.
  3     *        *        *     Request timed out.
  4    27 ms    10 ms     9 ms  lcmaaa-az-in-x0e.1e100.net [2404:6800:4007:836::200e]

Trace complete.
```
## 4.netstat
```
## C:\Users\acer>netstat -an

Active Connections

  Proto  Local Address          Foreign Address        State
  TCP    0.0.0.0:80             0.0.0.0:0              LISTENING
  TCP    0.0.0.0:135            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:445            0.0.0.0:0              LISTENING
  TCP    0.0.0.0:1309           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:4343           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:4449           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:5040           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:5141           0.0.0.0:0              LISTENING
  TCP    0.0.0.0:46760          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49664          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49665          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49666          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49667          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49668          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:49677          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:58995          0.0.0.0:0              LISTENING
  TCP    127.0.0.1:5141         127.0.0.1:57729        ESTABLISHED
  TCP    127.0.0.1:7768         0.0.0.0:0              LISTENING
  TCP    127.0.0.1:9993         0.0.0.0:0              LISTENING
  TCP    127.0.0.1:15152        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:19443        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46753        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46934        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46935        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46935        127.0.0.1:51370        ESTABLISHED
  TCP    127.0.0.1:46936        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46936        127.0.0.1:49686        ESTABLISHED
  TCP    127.0.0.1:46937        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:46937        127.0.0.1:49687        ESTABLISHED
  TCP    127.0.0.1:49669        127.0.0.1:49670        ESTABLISHED
  TCP    127.0.0.1:49670        127.0.0.1:49669        ESTABLISHED
  TCP    127.0.0.1:49675        127.0.0.1:49676        ESTABLISHED
  TCP    127.0.0.1:49676        127.0.0.1:49675        ESTABLISHED
  TCP    127.0.0.1:49678        127.0.0.1:49679        ESTABLISHED
  TCP    127.0.0.1:49679        127.0.0.1:49678        ESTABLISHED
  TCP    127.0.0.1:49680        127.0.0.1:49681        ESTABLISHED
  TCP    127.0.0.1:49681        127.0.0.1:49680        ESTABLISHED
  TCP    127.0.0.1:49682        127.0.0.1:49683        ESTABLISHED
  TCP    127.0.0.1:49683        127.0.0.1:49682        ESTABLISHED
  TCP    127.0.0.1:49684        127.0.0.1:49685        ESTABLISHED
  TCP    127.0.0.1:49685        127.0.0.1:49684        ESTABLISHED
  TCP    127.0.0.1:49686        127.0.0.1:46936        ESTABLISHED
  TCP    127.0.0.1:49687        127.0.0.1:46937        ESTABLISHED
  TCP    127.0.0.1:51364        127.0.0.1:51365        ESTABLISHED
  TCP    127.0.0.1:51365        127.0.0.1:51364        ESTABLISHED
  TCP    127.0.0.1:51366        127.0.0.1:51367        ESTABLISHED
  TCP    127.0.0.1:51367        127.0.0.1:51366        ESTABLISHED
  TCP    127.0.0.1:51368        127.0.0.1:51369        ESTABLISHED
  TCP    127.0.0.1:51369        127.0.0.1:51368        ESTABLISHED
  TCP    127.0.0.1:51370        127.0.0.1:46935        ESTABLISHED
  TCP    127.0.0.1:51779        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:51780        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:51781        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:51782        0.0.0.0:0              LISTENING
  TCP    127.0.0.1:53322        127.0.0.1:58995        ESTABLISHED
  TCP    127.0.0.1:54469        127.0.0.1:58995        ESTABLISHED
  TCP    127.0.0.1:57729        127.0.0.1:5141         ESTABLISHED
  TCP    127.0.0.1:58932        127.0.0.1:58995        ESTABLISHED
  TCP    127.0.0.1:58995        127.0.0.1:53322        ESTABLISHED
  TCP    127.0.0.1:58995        127.0.0.1:54469        ESTABLISHED
  TCP    127.0.0.1:58995        127.0.0.1:58932        ESTABLISHED
  TCP    169.254.235.4:139      0.0.0.0:0              LISTENING
  TCP    [::]:80                [::]:0                 LISTENING
  TCP    [::]:135               [::]:0                 LISTENING
  TCP    [::]:445               [::]:0                 LISTENING
  TCP    [::]:4343              [::]:0                 LISTENING
  TCP    [::]:4449              [::]:0                 LISTENING
  TCP    [::]:5141              [::]:0                 LISTENING
  TCP    [::]:46760             [::]:0                 LISTENING
  TCP    [::]:49664             [::]:0                 LISTENING
  TCP    [::]:49665             [::]:0                 LISTENING
  TCP    [::]:49666             [::]:0                 LISTENING
  TCP    [::]:49667             [::]:0                 LISTENING
  TCP    [::]:49668             [::]:0                 LISTENING
  TCP    [::]:49677             [::]:0                 LISTENING
  TCP    [::]:58995             [::]:0                 LISTENING
  TCP    [::1]:15161            [::]:0                 LISTENING
  TCP    [::1]:15161            [::1]:53323            ESTABLISHED
  TCP    [::1]:15161            [::1]:57734            ESTABLISHED
  TCP    [::1]:15161            [::1]:59266            TIME_WAIT
  TCP    [::1]:15161            [::1]:65450            TIME_WAIT
  TCP    [::1]:15161            [::1]:65451            ESTABLISHED
  TCP    [::1]:53323            [::1]:15161            ESTABLISHED
  TCP    [::1]:57734            [::1]:15161            ESTABLISHED
  TCP    [::1]:65451            [::1]:15161            ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:49411  [2603:1040:a06:6::]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:50540  [2603:1047:1:88::80]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:51735  [64:ff9b::34b6:8d3f]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:53929  [2603:1063:27:2::14]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:54378  [64:ff9b::34b6:8d3f]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:54713  [64:ff9b::330b:c031]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:54731  [2a06:98c1:3107::6812:2715]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:55085  [2603:1061:14:155::1]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:55379  [2603:1046:c06:c71::2]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:55380  [2603:1046:c06:c71::2]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:55381  [2603:1046:c06:c71::2]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:55382  [2603:1046:c06:c71::2]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:55389  [64:ff9b::14be:91a0]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:57739  [2603:1040:5:3::a]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:57742  [2603:1040:a06:6::2]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:58607  [2404:6800:4003:c1a::bc]:5228  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:58857  [64:ff9b::14be:918c]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:59267  [64:ff9b::14be:918c]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:59268  [64:ff9b::14be:918c]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:59269  [64:ff9b::14be:918c]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:59270  [64:ff9b::14be:918c]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:59567  [2603:1046:2000:90::4]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:61885  [2620:1ec:50::17]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:63908  [64:ff9b::23d9:11c4]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:64156  [2603:1063:2001:1916::365:ff1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:64157  [2603:1063:2001:1916::365:ff1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:64158  [2603:1063:2001:1916::365:ff1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:64159  [2603:1063:2001:1916::365:ff1]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:64480  [2603:1061:10:1::13]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:64511  [64:ff9b::34b6:8d3f]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:64844  [2603:1046:2000:90::3]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:64888  [2620:1ec:a92::156]:443  TIME_WAIT
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:65267  [2620:1ec:33:1::11]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:65326  [64:ff9b::14bd:ad1a]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:65327  [64:ff9b::330b:c033]:443  ESTABLISHED
  TCP    [2403:8600:c090:42:0:401:9bfa:fd9f]:65449  [2600:140f:6::172c:ae1]:443  ESTABLISHED
  UDP    0.0.0.0:5050           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5353           *:*
  UDP    0.0.0.0:5355           *:*
  UDP    0.0.0.0:49665          0.0.32.3:443
  UDP    0.0.0.0:51777          *:*
  UDP    0.0.0.0:54065          104.18.32.47:443
  UDP    0.0.0.0:55613          *:*
  UDP    0.0.0.0:56129          *:*
  UDP    0.0.0.0:56673          0.0.0.84:443
  UDP    127.0.0.1:1309         127.0.0.1:1309
  UDP    127.0.0.1:1900         *:*
  UDP    127.0.0.1:49664        127.0.0.1:49664
  UDP    127.0.0.1:56128        *:*
  UDP    127.0.0.1:62187        *:*
  UDP    169.254.235.4:137      *:*
  UDP    169.254.235.4:138      *:*
  UDP    169.254.235.4:1900     *:*
  UDP    169.254.235.4:62186    *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5353              *:*
  UDP    [::]:5355              *:*
  UDP    [::]:49665             [2404:6800:4007:808::2003]:443
  UDP    [::]:51777             *:*
  UDP    [::]:54065             [2a06:98c1:3100::6812:202f]:443
  UDP    [::]:55613             *:*
  UDP    [::]:56673             [2404:6800:4000:1025::54]:443
  UDP    [::1]:1900             *:*
  UDP    [::1]:62185            *:*
  UDP    [fe80::d30d:62b0:7886:c7b9%18]:1900  *:*
  UDP    [fe80::d30d:62b0:7886:c7b9%18]:62184  *:*
```
## 5.nslookup
```

## C:\Users\acer>nslookup google.com
Server:  UnKnown
Address:  2403:8600:c090:42:a000::200

Non-authoritative answer:
Name:    google.com
Addresses:  2404:6800:4007:836::200e
          142.251.221.110
```
## 6.hostname
```
## C:\Users\acer>hostname
TMP215-75-G2
```
## 7. arp -a
```
## C:\Users\acer>arp -a

Interface: 169.254.235.4 --- 0x12
  Internet Address      Physical Address      Type
  169.254.40.3          fc-6d-77-8a-7e-92     dynamic
  169.254.51.236        fc-6d-77-89-b0-ca     dynamic
  169.254.55.110        fc-6d-77-6f-d3-08     dynamic
  169.254.248.246       fc-6d-77-6f-b7-e2     dynamic
  169.254.255.255       ff-ff-ff-ff-ff-ff     static
  224.0.0.2             01-00-5e-00-00-02     static
  224.0.0.22            01-00-5e-00-00-16     static
  224.0.0.251           01-00-5e-00-00-fb     static
  224.0.0.252           01-00-5e-00-00-fc     static
  239.255.255.250       01-00-5e-7f-ff-fa     static
  255.255.255.255       ff-ff-ff-ff-ff-ff     static
```
## 8.route print
```
## C:\Users\acer>route print
===========================================================================
Interface List
  7...fc 6d 77 6d 9c e7 ......Microsoft Wi-Fi Direct Virtual Adapter
 11...fe 6d 77 6d 9c e6 ......Microsoft Wi-Fi Direct Virtual Adapter #2
 18...fc 6d 77 6d 9c e6 ......Intel(R) Wi-Fi 6E AX211 160MHz
  9...74 d4 dd cf 7a e3 ......Realtek PCIe GbE Family Controller
  1...........................Software Loopback Interface 1
===========================================================================

IPv4 Route Table
===========================================================================
Active Routes:
Network Destination        Netmask          Gateway       Interface  Metric
        127.0.0.0        255.0.0.0         On-link         127.0.0.1    331
        127.0.0.1  255.255.255.255         On-link         127.0.0.1    331
  127.255.255.255  255.255.255.255         On-link         127.0.0.1    331
      169.254.0.0      255.255.0.0         On-link     169.254.235.4    291
    169.254.235.4  255.255.255.255         On-link     169.254.235.4    291
  169.254.255.255  255.255.255.255         On-link     169.254.235.4    291
        224.0.0.0        240.0.0.0         On-link         127.0.0.1    331
        224.0.0.0        240.0.0.0         On-link     169.254.235.4    291
  255.255.255.255  255.255.255.255         On-link         127.0.0.1    331
  255.255.255.255  255.255.255.255         On-link     169.254.235.4    291
===========================================================================
Persistent Routes:
  None

IPv6 Route Table
===========================================================================
Active Routes:
 If Metric Network Destination      Gateway
 18    291 ::/0                     fe80::eedd:24ff:fe3d:ced5
  1    331 ::1/128                  On-link
 18    291 2403:8600:c090:42::/84   On-link
 18    291 2403:8600:c090:42:0:401:9bfa:fd9f/128
                                    On-link
 18    291 fe80::/64                On-link
 18    291 fe80::d30d:62b0:7886:c7b9/128
                                    On-link
  1    331 ff00::/8                 On-link
 18    291 ff00::/8                 On-link
===========================================================================
Persistent Routes:
  None
```
## 9.getmac
```
## C:\Users\acer>getmac

Physical Address    Transport Name
=================== ==========================================================
FC-6D-77-6D-9C-E6   \Device\Tcpip_{EDF10F09-987F-4CBD-B529-CFCDF3C4EA9F}
74-D4-DD-CF-7A-E3   Media disconnected
```
## 10.curl
```
## C:\Users\acer>curl https://example.com
<!doctype html><html lang="en"><head><title>Example Domain</title><meta name="viewport" content="width=device-width, initial-scale=1"><style>body{background:#eee;width:60vw;margin:15vh auto;font-family:system-ui,sans-serif}h1{font-size:1.5em}div{opacity:0.8}a:link,a:visited{color:#348}</style></head><body><div><h1>Example Domain</h1><p>This domain is for use in documentation examples without needing permission. Avoid use in operations.</p><p><a href="https://iana.org/domains/example">Learn more</a></p></div></body></html>
```
## Result
Thus Execution of Network commands Performed 
