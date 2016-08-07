# /proc/net/snmp

## Ip

### Forwarding

### DefaultTTL

### InReceives

### InHdrErrors

### InAddrErrors

### ForwDatagrams

### InUnknownProtos

### InDiscards

### InDelivers

### OutRequests

### OutDiscards

### OutNoRoutes

### ReasmTimeout

### ReasmReqds

### ReasmOKs

### ReasmFails

### FragOKs

### FragFails

### FragCreates

## Icmp

### InMsgs

### InErrors

### InCsumErrors

### InDestUnreachs

### InTimeExcds

### InParmProbs

### InSrcQuenchs

### InRedirects

### InEchos

### InEchoReps

### InTimestamps

### InTimestampReps

### InAddrMasks

### InAddrMaskReps

### OutMsgs

### OutErrors

### OutDestUnreachs

### OutTimeExcds

### OutParmProbs

### OutSrcQuenchs

### OutRedirects

### OutEchos

### OutEchoReps

### OutTimestamps

### OutTimestampReps

### OutAddrMasks

### OutAddrMaskReps

## Icmp

### InType0

### InType3

### InType4

### InType5

### InType8

### InType11

### OutType0

### OutType3

## Tcp

### RtoAlgorithm

### RtoMin

### RtoMax

### MaxConn

### ActiveOpens

### PassiveOpens

### AttemptFails

### EstabResets

### CurrEstab

established TCP connection counter. when non-TCP_ESTABLISHED state is changed
to TCP_ESTABLISHED state, it is increased by 1. when TCP_ESTABLISHED state is
changed to non-TCP_ESTABLISHED state, it is decreased by 1.

see also: net/ipv4/tcp.c `tcp_set_state()`, TCP_CLOSE, TCP_SYN_SENT,
TCP_CLOSE_WAIT, TCP_CLOSING, TCP_ESTABLISHED, TCP_SYN_RECV, TCP_FIN_WAIT2,
IPv6?

### InSegs

### OutSegs

### RetransSegs

### InErrs

### OutRsts

### InCsumErrors

## Udp

### InDatagrams

### NoPorts

### InErrors

### OutDatagrams

### RcvbufErrors

### SndbufErrors

### InCsumErrors

## UdpLite

### InDatagrams

### NoPorts

### InErrors

### OutDatagrams

### RcvbufErrors

### SndbufErrors

### InCsumErrors

