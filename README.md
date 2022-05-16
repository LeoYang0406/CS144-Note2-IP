# IP services

## 4 Properties:
    Datagram: individually routed packets, hop-by-hop routing
    Unreliable: packets may be dropped
    Best effort: 只在必要的时候才会make errors like dropping packets
    Connectionless: No per-flow state. Packets may be mis-sequenced.
    
## 为什么IP is so simple:
    1. Simple means faster & lower cost
    2. End-to-end principle
    3. Allow a variety of reliable services built on top(因为即使IP能够保证每一次传输的完整，这个特性对一些application并非是有利的)
    3. 能够work over任何link layers
    
    对于不需要保证数据完整性和顺序的应用，可以用UDP(user datagram protocol) instead of TCP
    
## IP的五个特性:
    1. IP tries to prenvent packets from looping forever
    2. IP will fragment packets if they are too long
    3. IP uses a header checksum to reduce the chances of delivering datagram to the wrong destination
    4. Allows for new versions of IP
    5. Allows for new options to be added to the header
