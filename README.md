# IP services

## 4 Properties:
   Datagram: individually routed packets, hop-by-hop routing
   Unreliable: packets may be dropped
   Best effort: 只在必要的时候才会make errors like dropping packets
   Connectionless: No per-flow state. Packets may be mis-sequenced.
    
## TCP/IP的关系:
    TCP是transport layer的transmission control protocol
    IP是network layer的Internet protocol
    因为Internet protocol不保证datagram以及传输的完整性
    所以要用到TCP above the head of IP，来保证得到correct and in-order data
    TCP: make sure the data sent by one appliation to another is correctly delivered in right order.
    
    对于不需要保证数据完整性和顺序的应用，可以用UDP(user datagram protocol) instead of TCP
    
## IP的独特性:
    IP 是 'thin wrist'
    因为IP是一定要被用到的（if you want to use the Internet）
    但是Link layer和transport layer都有很多其他不同的选择
    
