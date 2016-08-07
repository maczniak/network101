# ss

(Linux-specific)

## -s, --summary

This option uses informations in `/proc/net/sockstat`, `/proc/net/sockstat6`,
`/proc/net/snmp` and `/proc/slabinfo`.

output:
```
Total: 165 (kernel 450)
       (1)         (11)
TCP:   64 (estab 55, closed 0, orphaned 0, synrecv 0, timewait 0/0), ports 0
      (4+5)     (10)    (4+5-2-2')     (3)        (0)         (4)(0)      (0?)

Transport Total     IP        IPv6
*         450       -         -
          (11)
RAW       0         0         0
        (8+8')     (8)       (8')
UDP       3         2         1
        (7+7')     (7)       (7')
TCP       64        22        42
        (2+2')      (2)      (2')
INET      67        24        43
          (RAW  +  UDP  +   TCP)
FRAG      0         0         0
        (9+9')     (9)       (9')
```

/proc/net/sockstat:
```
sockets: used 165
              (1)
TCP: inuse 22 orphan 0 tw 0 alloc 64 mem 7
           (2)      (3)  (4)      (5)   (6)
UDP: inuse 2 mem 0
          (7)
UDPLITE: inuse 0
RAW: inuse 0
          (8)
FRAG: inuse 0 memory 0
           (9)
```

/proc/net/sockstat6:
```
TCP6: inuse 42
           (2')
UDP6: inuse 1
           (7')
UDPLITE6: inuse 0
RAW6: inuse 0
           (8')
FRAG6: inuse 0 memory 0
            (9')
```

(0): always 0<br>
(10): `Tcp` `[CurrEstab](../kernel_info/proc_net_snmp.md#currestab)` in `/proc/net/snmp`<br>
(11): `sock_inode_cache` `<active_objs>` in `/proc/slabinfo`

## links

from [iproute2](../packages/iproute2.md)-3.11.0

