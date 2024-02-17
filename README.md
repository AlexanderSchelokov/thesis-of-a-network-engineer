Тестирование

Проверка STP, HSRP. Роль Root bridge и HSRP-active на одном устройстве. Команды: show spanning-tree, show standby на этом устройстве.

```
core1#show spanning-tree
VLAN0001
  Spanning tree enabled protocol ieee
  Root ID    Priority    24577
             Address     0060.3E91.5590
             This bridge is the root
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec

  Bridge ID  Priority    24577  (priority 24576 sys-id-ext 1)
             Address     0060.3E91.5590
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec
             Aging Time  20

Interface        Role Sts Cost      Prio.Nbr Type
---------------- ---- --- --------- -------- --------------------------------
Fa0/5            Desg FWD 19        128.5    P2p
Fa0/1            Desg FWD 19        128.1    P2p
Fa0/2            Desg FWD 19        128.2    P2p
Po1              Desg FWD 3         128.27   Shr

VLAN0050
  Spanning tree enabled protocol ieee
  Root ID    Priority    32818
             Address     0001.6485.315D
             Cost        19
             Port        5(FastEthernet0/5)
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec

  Bridge ID  Priority    32818  (priority 32768 sys-id-ext 50)
             Address     0060.3E91.5590
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec
             Aging Time  20

Interface        Role Sts Cost      Prio.Nbr Type
---------------- ---- --- --------- -------- --------------------------------
Fa0/5            Root FWD 19        128.5    P2p
Fa0/1            Desg FWD 19        128.1    P2p
Fa0/2            Desg FWD 19        128.2    P2p
Po1              Altn BLK 3         128.27   Shr

VLAN0100
  Spanning tree enabled protocol ieee
  Root ID    Priority    24676
             Address     0060.3E91.5590
             This bridge is the root
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec

  Bridge ID  Priority    24676  (priority 24576 sys-id-ext 100)
             Address     0060.3E91.5590
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec
             Aging Time  20

Interface        Role Sts Cost      Prio.Nbr Type
---------------- ---- --- --------- -------- --------------------------------
Fa0/5            Desg FWD 19        128.5    P2p
Fa0/1            Desg FWD 19        128.1    P2p
Fa0/2            Desg FWD 19        128.2    P2p
Po1              Desg FWD 3         128.27   Shr

VLAN0200
  Spanning tree enabled protocol ieee
  Root ID    Priority    24776
             Address     0060.3E91.5590
             This bridge is the root
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec

  Bridge ID  Priority    24776  (priority 24576 sys-id-ext 200)
             Address     0060.3E91.5590
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec
             Aging Time  20

Interface        Role Sts Cost      Prio.Nbr Type
---------------- ---- --- --------- -------- --------------------------------
Fa0/5            Desg FWD 19        128.5    P2p
Fa0/1            Desg FWD 19        128.1    P2p
Fa0/2            Desg FWD 19        128.2    P2p
Po1              Desg FWD 3         128.27   Shr

VLAN0201
  Spanning tree enabled protocol ieee
  Root ID    Priority    24777
             Address     0060.3E91.5590
             This bridge is the root
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec

  Bridge ID  Priority    24777  (priority 24576 sys-id-ext 201)
             Address     0060.3E91.5590
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec
             Aging Time  20

Interface        Role Sts Cost      Prio.Nbr Type
---------------- ---- --- --------- -------- --------------------------------
Fa0/5            Desg FWD 19        128.5    P2p
Fa0/1            Desg FWD 19        128.1    P2p
Fa0/2            Desg FWD 19        128.2    P2p
Po1              Desg FWD 3         128.27   Shr

VLAN0300
  Spanning tree enabled protocol ieee
  Root ID    Priority    24876
             Address     0060.3E91.5590
             This bridge is the root
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec

  Bridge ID  Priority    24876  (priority 24576 sys-id-ext 300)
             Address     0060.3E91.5590
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec
             Aging Time  20

Interface        Role Sts Cost      Prio.Nbr Type
---------------- ---- --- --------- -------- --------------------------------
Fa0/5            Desg FWD 19        128.5    P2p
Fa0/1            Desg FWD 19        128.1    P2p
Fa0/2            Desg FWD 19        128.2    P2p
Po1              Desg FWD 3         128.27   Shr

VLAN0400
  Spanning tree enabled protocol ieee
  Root ID    Priority    24976
             Address     0060.3E91.5590
             This bridge is the root
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec

  Bridge ID  Priority    24976  (priority 24576 sys-id-ext 400)
             Address     0060.3E91.5590
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec
             Aging Time  20

Interface        Role Sts Cost      Prio.Nbr Type
---------------- ---- --- --------- -------- --------------------------------
Fa0/5            Desg FWD 19        128.5    P2p
Fa0/1            Desg FWD 19        128.1    P2p
Fa0/2            Desg FWD 19        128.2    P2p
Po1              Desg FWD 3         128.27   Shr

VLAN0401
  Spanning tree enabled protocol ieee
  Root ID    Priority    24977
             Address     0060.3E91.5590
             This bridge is the root
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec

  Bridge ID  Priority    24977  (priority 24576 sys-id-ext 401)
             Address     0060.3E91.5590
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec
             Aging Time  20

Interface        Role Sts Cost      Prio.Nbr Type
---------------- ---- --- --------- -------- --------------------------------
Fa0/5            Desg FWD 19        128.5    P2p
Fa0/1            Desg FWD 19        128.1    P2p
Fa0/2            Desg FWD 19        128.2    P2p
Po1              Desg FWD 3         128.27   Shr

VLAN0500
  Spanning tree enabled protocol ieee
  Root ID    Priority    25076
             Address     0060.3E91.5590
             This bridge is the root
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec

  Bridge ID  Priority    25076  (priority 24576 sys-id-ext 500)
             Address     0060.3E91.5590
             Hello Time  2 sec  Max Age 20 sec  Forward Delay 15 sec
             Aging Time  20

Interface        Role Sts Cost      Prio.Nbr Type
---------------- ---- --- --------- -------- --------------------------------
Fa0/5            Desg FWD 19        128.5    P2p
Fa0/1            Desg FWD 19        128.1    P2p
Fa0/2            Desg FWD 19        128.2    P2p
Po1              Desg FWD 3         128.27   Shr
```
```
core1#  show standby
Vlan50 - Group 1
  State is Active
    5 state changes, last state change 00:00:18
  Virtual IP address is 192.168.1.1
  Active virtual MAC address is 0000.0C07.AC01
    Local virtual MAC address is 0000.0C07.AC01 (v1 default)
  Hello time 3 sec, hold time 10 sec
    Next hello sent in 2.021 secs
  Preemption enabled
  Active router is local
  Standby router is 192.168.1.253, priority 50 (expires in 7 sec)
  Priority 110 (configured 110)
  Group name is hsrp-Vl5-1 (default)
Vlan100 - Group 1
  State is Active
    5 state changes, last state change 00:00:17
  Virtual IP address is 192.168.0.1
  Active virtual MAC address is 0000.0C07.AC01
    Local virtual MAC address is 0000.0C07.AC01 (v1 default)
  Hello time 3 sec, hold time 10 sec
    Next hello sent in 1.067 secs
  Preemption enabled
  Active router is local
  Standby router is unknown
  Priority 110 (configured 110)
  Group name is hsrp-Vl1-1 (default)
Vlan200 - Group 1
  State is Active
    5 state changes, last state change 00:00:28
  Virtual IP address is 192.168.2.1
  Active virtual MAC address is 0000.0C07.AC01
    Local virtual MAC address is 0000.0C07.AC01 (v1 default)
  Hello time 3 sec, hold time 10 sec
    Next hello sent in 2.908 secs
  Preemption enabled
  Active router is local
  Standby router is 192.168.2.253
  Priority 110 (configured 110)
  Group name is hsrp-Vl2-1 (default)
Vlan300 - Group 1
  State is Active
    6 state changes, last state change 00:00:28
  Virtual IP address is 192.168.3.1
  Active virtual MAC address is 0000.0C07.AC01
    Local virtual MAC address is 0000.0C07.AC01 (v1 default)
  Hello time 3 sec, hold time 10 sec
    Next hello sent in 0.132 secs
  Preemption enabled
  Active router is local
  Standby router is 192.168.3.253
  Priority 110 (configured 110)
  Group name is hsrp-Vl3-1 (default)
Vlan400 - Group 1
  State is Active
    5 state changes, last state change 00:00:17
  Virtual IP address is 192.168.4.1
  Active virtual MAC address is 0000.0C07.AC01
    Local virtual MAC address is 0000.0C07.AC01 (v1 default)
  Hello time 3 sec, hold time 10 sec
    Next hello sent in 1.865 secs
  Preemption enabled
  Active router is local
  Standby router is 192.168.4.253, priority 50 (expires in 8 sec)
  Priority 110 (configured 110)
  Group name is hsrp-Vl4-1 (default)
Vlan500 - Group 1
  State is Active
    6 state changes, last state change 00:00:32
  Virtual IP address is 192.168.5.1
  Active virtual MAC address is 0000.0C07.AC01
    Local virtual MAC address is 0000.0C07.AC01 (v1 default)
  Hello time 3 sec, hold time 10 sec
    Next hello sent in 0.343 secs
  Preemption enabled
  Active router is local
  Standby router is 192.168.5.126, priority 50 (expires in 6 sec)
  Priority 110 (configured 110)
  Group name is hsrp-Vl5-1 (default)
```


Проверка маршрутизации на коммутаторах ядра. Show ip route. Должен присутствовать маршрут по-умолчанию и маршруты до интерфейсов ASA и бордеров.

```
core1#Show ip route
Codes: C - connected, S - static, I - IGRP, R - RIP, M - mobile, B - BGP
       D - EIGRP, EX - EIGRP external, O - OSPF, IA - OSPF inter area
       N1 - OSPF NSSA external type 1, N2 - OSPF NSSA external type 2
       E1 - OSPF external type 1, E2 - OSPF external type 2, E - EGP
       i - IS-IS, L1 - IS-IS level-1, L2 - IS-IS level-2, ia - IS-IS inter area
       * - candidate default, U - per-user static route, o - ODR
       P - periodic downloaded static route

Gateway of last resort is 10.10.10.2 to network 0.0.0.0

     10.0.0.0/30 is subnetted, 1 subnets
C       10.10.10.0 is directly connected, FastEthernet0/4
     20.0.0.0/30 is subnetted, 1 subnets
O       20.20.20.0 [110/2] via 10.10.10.2, 00:27:09, FastEthernet0/4
     30.0.0.0/30 is subnetted, 1 subnets
O       30.30.30.0 [110/2] via 192.168.1.253, 00:26:34, Vlan50
                   [110/2] via 192.168.2.253, 00:26:34, Vlan200
                   [110/2] via 192.168.3.253, 00:26:34, Vlan300
                   [110/2] via 192.168.4.253, 00:26:34, Vlan400
                   [110/2] via 192.168.5.126, 00:26:34, Vlan500
     192.168.0.0/25 is subnetted, 1 subnets
C       192.168.0.0 is directly connected, Vlan100
C    192.168.1.0/24 is directly connected, Vlan50
C    192.168.2.0/24 is directly connected, Vlan200
C    192.168.3.0/24 is directly connected, Vlan300
C    192.168.4.0/24 is directly connected, Vlan400
     192.168.5.0/25 is subnetted, 1 subnets
C       192.168.5.0 is directly connected, Vlan500
O*IA 0.0.0.0/0 [110/3] via 10.10.10.2, 00:27:09, FastEthernet0/4
```



Проверка LAG на коммутаторах ядра show etherchannel summary.
```
core1#show etherchannel
                Channel-group listing:
                ----------------------

Group: 1
----------
Group state = L2
Ports: 2 Maxports = 16
Port-channels: 1 Max Port-channels = 16
Protocol:   LACP
```


Маршрутизация на бордерах sh ip route. В таблице маршрутизации должны присутствовать bgp-маршруты от провайдера, ospf-маршруты до внутренних подсетей ЦО и филиала.

```
Router#sh ip route 
Codes: L - local, C - connected, S - static, R - RIP, M - mobile, B - BGP
       D - EIGRP, EX - EIGRP external, O - OSPF, IA - OSPF inter area
       N1 - OSPF NSSA external type 1, N2 - OSPF NSSA external type 2
       E1 - OSPF external type 1, E2 - OSPF external type 2, E - EGP
       i - IS-IS, L1 - IS-IS level-1, L2 - IS-IS level-2, ia - IS-IS inter area
       * - candidate default, U - per-user static route, o - ODR
       P - periodic downloaded static route

Gateway of last resort is 172.1.0.1 to network 0.0.0.0

     1.0.0.0/8 is variably subnetted, 2 subnets, 2 masks
C       1.1.1.0/30 is directly connected, Tunnel1
L       1.1.1.1/32 is directly connected, Tunnel1
     2.0.0.0/30 is subnetted, 1 subnets
O IA    2.2.2.0/30 [110/1001] via 50.50.50.2, 4294967293:4294967288:4294967248, GigabitEthernet0/1/0
     5.0.0.0/32 is subnetted, 1 subnets
C       5.5.5.5/32 is directly connected, Loopback0
     8.0.0.0/24 is subnetted, 1 subnets
B       8.8.8.0/24 [20/0] via 172.1.0.1, 00:00:00
     10.0.0.0/30 is subnetted, 1 subnets
O       10.10.10.0/30 [110/2] via 20.20.20.2, 00:28:32, GigabitEthernet0/1
     20.0.0.0/8 is variably subnetted, 2 subnets, 2 masks
C       20.20.20.0/30 is directly connected, GigabitEthernet0/1
L       20.20.20.1/32 is directly connected, GigabitEthernet0/1
     30.0.0.0/30 is subnetted, 1 subnets
O       30.30.30.0/30 [110/4] via 20.20.20.2, 00:28:22, GigabitEthernet0/1
     40.0.0.0/30 is subnetted, 1 subnets
O IA    40.40.40.0/30 [110/2] via 50.50.50.2, 4294967293:4294967288:4294967248, GigabitEthernet0/1/0
     50.0.0.0/8 is variably subnetted, 2 subnets, 2 masks
C       50.50.50.0/30 is directly connected, GigabitEthernet0/1/0
L       50.50.50.1/32 is directly connected, GigabitEthernet0/1/0
     172.1.0.0/16 is variably subnetted, 2 subnets, 2 masks
C       172.1.0.0/30 is directly connected, GigabitEthernet0/0
L       172.1.0.2/32 is directly connected, GigabitEthernet0/0
     172.2.0.0/30 is subnetted, 1 subnets
B       172.2.0.0/30 [20/0] via 172.1.0.1, 00:00:00
     172.3.0.0/30 is subnetted, 1 subnets
B       172.3.0.0/30 [20/0] via 172.1.0.1, 00:00:00
O    192.168.1.0/24 [110/3] via 20.20.20.2, 00:28:02, GigabitEthernet0/1
O    192.168.2.0/24 [110/3] via 20.20.20.2, 00:28:02, GigabitEthernet0/1
O    192.168.3.0/24 [110/3] via 20.20.20.2, 00:27:52, GigabitEthernet0/1
O    192.168.4.0/24 [110/3] via 20.20.20.2, 00:27:52, GigabitEthernet0/1
     192.168.5.0/25 is subnetted, 1 subnets
O       192.168.5.0/25 [110/3] via 20.20.20.2, 00:28:32, GigabitEthernet0/1
     192.168.8.0/25 is subnetted, 1 subnets
O       192.168.8.0/25 [110/1001] via 1.1.1.2, 4294967294:4294967271:4294967242, Tunnel1
O    192.168.9.0/24 [110/1001] via 1.1.1.2, 4294967294:4294967256:4294967260, Tunnel1
     192.168.11.0/26 is subnetted, 1 subnets
O       192.168.11.0/26 [110/1001] via 1.1.1.2, 4294967294:4294967271:4294967242, Tunnel1
O    192.168.12.0/24 [110/1001] via 1.1.1.2, 4294967294:4294967271:4294967242, Tunnel1
S*   0.0.0.0/0 [10/0] via 172.1.0.1
```

Туннель CAPWAP на БЛВС ТД в статусе Connected, с ноутбуков есть связь с 8.8.8.8.

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/57f1e64b-c482-451a-a1bd-b5cd01e1dce2)

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/1bdab6cb-1129-4337-8cc6-eea675a78461)


Телефонные аппараты зарегестрированы на VoIP сервере, прозвон с одного на другой работает.

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/92465b77-0e90-403a-a90c-a9a5ad5db8c7)

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/b099fa39-437a-4bd1-bea5-2d24838b93dc)



На все сетевые устройства можно попасть по учётной записи tacacs+ сервера.
![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/210d2d47-e9a0-4ee7-a9c0-e44d12490108)

Время на устройствах синхронизировано. Show ntp status.

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/e2882132-616a-4ca8-b40e-db8ca56285a7)


С 8.8.8.8 есть доступ к web-серверу в DMZ. Обратный доступ тоже есть. Проверять доступ необходимо браузером.

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/90b6756e-be07-4c6e-aa68-2f1a5b5cfd7e)

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/d07e5c7f-d64f-41f1-bb0d-fb7ec4b9ffaa)


Отключение одного из каналов связи не приводит к потере доступа в интернет с пользовательских ПК(ping до сервера 8.8.8.8).

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/9ad8b12f-8fa5-4ed9-8144-d3266d45805a)

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/3acfb597-eceb-47e0-b78c-f807e2e169ce)


Выход из строя одного из коммутаторов ядра, межсетевого экрана или бордер роутера не приводит к потере доступа в интернет с пользовательских ПК(ping до сервера 8.8.8.8). Потеря доступа к web-серверу извне доспускается.

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/f6b67be2-73f6-4252-9fe2-779ec6a598be)

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/38bf755c-9b49-4b69-a395-fad60ee98c0d)

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/a7923cfe-ee1c-44cb-ad2a-927c2fe4e81c)


Ноутбуки не имеют доступа к внутренним сетям компании(ping svi users, mgmt, printer).

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/a9e46c2c-b305-4bff-8211-101842d0e780)


Устройства филиала имеют доступ только к внутренним сетям компании, не имеют выхода в интернет.

![image](https://github.com/AlexanderSchelokov/thesis-of-a-network-engineer/assets/121572590/dcf21afb-31a2-4f0e-9c18-219a8471d229)

