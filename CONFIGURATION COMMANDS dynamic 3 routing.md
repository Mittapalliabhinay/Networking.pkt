## ROUTER 1

B1R1>en

B1R1#show ip route

Codes: C - connected, S - static, I - IGRP, R - RIP, M - mobile, B - BGP

&#x20;      D - EIGRP, EX - EIGRP external, O - OSPF, IA - OSPF inter area

&#x20;      N1 - OSPF NSSA external type 1, N2 - OSPF NSSA external type 2

&#x20;      E1 - OSPF external type 1, E2 - OSPF external type 2, E - EGP

&#x20;      i - IS-IS, L1 - IS-IS level-1, L2 - IS-IS level-2, ia - IS-IS inter area

&#x20;      \* - candidate default, U - per-user static route, o - ODR

&#x20;      P - periodic downloaded static route



Gateway of last resort is not set



C    192.168.1.0/24 is directly connected, FastEthernet0/1

C    200.200.200.0/24 is directly connected, FastEthernet0/0

B1R1#config t

Enter configuration commands, one per line.  End with CNTL/Z.

B1R1(config)#router rip

B1R1(config-router)#ver 2

B1R1(config-router)#no auto-summary

B1R1(config-router)#network 192.168.1.0

B1R1(config-router)#network 200.200.200.0

B1R1(config-router)#exit

B1R1(config)#exit

B1R1#

%SYS-5-CONFIG\_I: Configured from console by console



B1R1#wr

Building configuration...

\[OK]

B1R1#

B1R1# 

B1R1#

## 

## ROUTER 2





HQR1>EN

HQR1#

HQR1#

HQR1#show ip route

Codes: C - connected, S - static, I - IGRP, R - RIP, M - mobile, B - BGP

&#x20;      D - EIGRP, EX - EIGRP external, O - OSPF, IA - OSPF inter area

&#x20;      N1 - OSPF NSSA external type 1, N2 - OSPF NSSA external type 2

&#x20;      E1 - OSPF external type 1, E2 - OSPF external type 2, E - EGP

&#x20;      i - IS-IS, L1 - IS-IS level-1, L2 - IS-IS level-2, ia - IS-IS inter area

&#x20;      \* - candidate default, U - per-user static route, o - ODR

&#x20;      P - periodic downloaded static route



Gateway of last resort is not set



&#x20;    100.0.0.0/24 is subnetted, 1 subnets

C       100.100.100.0 is directly connected, Serial0/0/0

C    192.168.0.0/24 is directly connected, FastEthernet0/1

C    200.200.200.0/24 is directly connected, FastEthernet0/0

HQR1#config t

Enter configuration commands, one per line.  End with CNTL/Z.

HQR1(config)#

HQR1(config)#router rip

HQR1(config-router)#ver 2

HQR1(config-router)#no auto-summary

HQR1(config-router)#network 100.100.100.0

HQR1(config-router)#network 192.168.0.0

HQR1(config-router)#network 200.200.200.0

HQR1(config-router)#exit

HQR1(config)#exit

HQR1#

%SYS-5-CONFIG\_I: Configured from console by console



HQR1#wr

Building configuration...

\[OK]

HQR1#

## 

## ROUTER 3



B2R1>en

B2R1#show ip route

Codes: C - connected, S - static, I - IGRP, R - RIP, M - mobile, B - BGP

&#x20;      D - EIGRP, EX - EIGRP external, O - OSPF, IA - OSPF inter area

&#x20;      N1 - OSPF NSSA external type 1, N2 - OSPF NSSA external type 2

&#x20;      E1 - OSPF external type 1, E2 - OSPF external type 2, E - EGP

&#x20;      i - IS-IS, L1 - IS-IS level-1, L2 - IS-IS level-2, ia - IS-IS inter area

&#x20;      \* - candidate default, U - per-user static route, o - ODR

&#x20;      P - periodic downloaded static route



Gateway of last resort is not set



&#x20;    100.0.0.0/24 is subnetted, 1 subnets

C       100.100.100.0 is directly connected, Serial0/0/0

C    192.168.2.0/24 is directly connected, FastEthernet0/1

B2R1#config t

Enter configuration commands, one per line.  End with CNTL/Z.

B2R1(config)#router rip

B2R1(config-router)#ver 2

B2R1(config-router)#no auto-summary

B2R1(config-router)#network 100.100.100.0

B2R1(config-router)#network 192.168.2.0

B2R1(config-router)#exit

B2R1(config)#exit

B2R1#

%SYS-5-CONFIG\_I: Configured from console by console



B2R1#wr

Building configuration...

\[OK]

B2R1#

B2R1#

