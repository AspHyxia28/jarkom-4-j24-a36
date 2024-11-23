| Name           | NRP        | Class     |
| ---            | ---        | ----------|
| 5025221018 | Mirza Zaki Rafii | Jaringan Komputer (A) |
| 5025231115 | Arkananta Masarief | Jaringan Komputer (A) |

<br>

<b> Letakkan link excel hasil perhitungan di sini </b>
<br>
<b> _Place the excel calculation results link here_ </b>
```
https://docs.google.com/spreadsheets/d/15Rw23_ngaQfGG8DYqEoMDUihwMsSpPlSIQfi8LSyqpA/edit?gid=0#gid=0
```


# Laporan Praktikum Modul 4 Non Terraform

## Prefix IP
Letakkan prefix IP yang digunakan di bawah:

_Put IP prefix used below:_
```
192.186.x.xxx
```

## Topology

- GNS3

  ![topologi](https://github.com/user-attachments/assets/f8cd1cfd-112d-4cd1-8537-33a11e58cd91)


- CPT

  ![topologi](https://github.com/user-attachments/assets/0c8b2afe-b3ae-403b-8cc9-9eb4260aa799)


<br>

## Routing

- Routing table

  ![image](https://github.com/user-attachments/assets/fe9fe6ca-a107-4d70-a0c6-aefc63330a9a)


- Route visualization in topology

  ![l](https://github.com/user-attachments/assets/c7872a4e-d3fc-4760-9b9e-d71d020c66eb)


<br>

## VLSM

### Tree

- Tree image
  
  `https://miro.com/app/board/uXjVLEZUw7A=/?share_link_id=882373901537`
  ![image](https://github.com/user-attachments/assets/486e9035-c1d3-4632-b565-0ef0786e8193)




- IP distribution table

  ![image](https://github.com/user-attachments/assets/e96e70a5-e21e-4e52-9738-b4c266a89207)
  



### Subnetting (If you use CPT)

`Put your subnetting configuration for each router, client, and server visualized in topology here || Masukkan konfigurasi untuk masing-masing router, client, dan server yang divisualisasikan pada topologi di sini`

### Subnetting (If you use GNS3)

Configuration to every router, client, and server for subnetting.

- Kamachi:

  ```
    auto eth0
    iface eth0 inet dhcp
    
    #A1
    auto eth1
    iface eth1 inet static
    	address 192.186.8.1
    	netmask 255.255.255.252
    
    #A6
    auto eth2
    iface eth2 inet static
    	address 192.186.8.13
    	netmask 255.255.255.252
    
    #A9
    auto eth3
    iface eth3 inet static
    	address 192.186.8.17
    	netmask 255.255.255.252
    
    #A16
    auto eth4
    iface eth4 inet static
    	address 192.186.8.37
    	netmask 255.255.255.252
    
    #A19
    auto eth5
    iface eth5 inet static
    	address 192.186.8.45
    	netmask 255.255.255.252
  ```

- Fiamma:

  ```
    #A19
    auto eth0 
    iface eth0 inet static
    	address 192.186.8.46
    	netmask 255.255.255.252
    
    #A20
    auto eth1
    iface eth1 inet static
    	address 192.186.14.1
    	netmask 255.255.254.0
  ```

- GoldenDawn:

  ```
    #A16
    auto eth0
    iface eth0 inet static
    	address 192.186.8.38
    	netmask 255.255.255.252
    
    #A17
    auto eth1
    iface eth1 inet static
    	address 192.186.8.41
    	netmask 255.255.255.252
    
    #A18
    auto eth2
    iface eth2 inet static
    	address 192.186.0.1
    	netmask 255.255.248.0
  ```

- Necessarius:

  ```
    #A9
    auto eth0
    iface eth0 inet static
    	address 192.186.8.18
    	netmask 255.255.255.252
    
    #A10
    auto eth1 
    iface eth1 inet static
    	address 192.186.8.21
    	netmask 255.255.255.252
    
    #A12
    auto eth2
    iface eth2 inet static
    	address 192.186.8.25
    	netmask 255.255.255.252

  ```

- Alice:

  ```
    #A6
    auto eth0
    iface eth0 inet static
    	address 192.186.8.14
    	netmask 255.255.255.252
    
    #A7
    auto eth1
    iface eth1 inet static
    	address 192.186.10.1
    	netmask 255.255.254.0
    
    
    
    ###Fuze
    #A7
    auto eth0
    iface eth0 inet static
    	address 192.186.10.3
    	netmask 255.255.254.0
    	gateway 192.186.10.1
  ```

- Kihara:

  ```
    #A1
    auto eth0
    iface eth0 inet static
    	address 192.186.8.2
    	netmask 255.255.255.252
    
    #A2
    auto eth1
    iface eth1 inet static
    	address 192.186.8.5
    	netmask 255.255.255.252
    
    #A3
    auto eth2
    iface eth2 inet static
    	address 192.186.8.9
    	netmask 255.255.255.252
  ```

- Vento:

  ```
    #A20
    auto eth0
    iface eth0 inet static
    	address 192.186.14.2
    	netmask 255.255.254.0
    
    #A21
    auto eth1
    iface eth1 inet static
    	address 192.186.8.225
    	netmask 255.255.255.224
  ```

- Terra:

  ```
    #A21
    auto eth0
    iface eth0 inet static
    	address 192.186.8.226
    	netmask 255.255.255.224
    	gateway 192.186.8.225
  ```

- Acqua:

  ```
    #A20
    auto eth0
    iface eth0 inet static
    	address 192.186.14.3
    	netmask 255.255.254.0
    	gateway 192.186.14.1
  ```

- Aiwass:

  ```
    #A18
    auto eth0
    iface eth0 inet static
    	address 192.186.4.1
    	netmask 255.255.248.0
    	gateway 192.186.0.1
  ```

- Aleister:

  ```
    #A18
    auto eth0
    iface eth0 inet static
    	address 192.186.0.2
    	netmask 255.255.248.0
    	gateway 192.186.0.1
  ```

- Mathers:

  ```
    #A17
    auto eth0
    iface eth0 inet static
    	address 192.186.8.42
    	netmask 255.255.255.252
    	gateway 192.186.8.41
  ```

- Coronzon:

  ```
    #A12
    auto eth0
    iface eth0 inet static
    	address 192.186.8.26
    	netmask 255.255.255.252
    
    #A13
    auto eth1
    iface eth1 inet static
    	address 192.186.8.29
    	netmask 255.255.255.252
    
    #A15
    auto eth2
    iface eth2 inet static
    	address 192.186.8.33
    	netmask 255.255.255.252
  ```

- Elizard:

  ```
    #A15
    auto eth0
    iface eth0 inet static
    	address 192.186.8.34
    	netmask 255.255.255.252
    	gateway 192.186.8.33
  ```

- Index:

  ```
    #A13
    auto eth0
    iface eth0 inet static
    	address 192.186.8.30
    	netmask 255.255.255.252
    
    #A14
    auto eth1
    iface eth1 inet static
    	address 192.186.8.177
    	netmask 255.255.255.240
  ```

- Magnus:

  ```
    #A14
    auto eth0 
    iface eth0 inet static
    	address 192.186.8.178
    	netmask 255.255.255.240
    	gateway 192.186.8.177
  ```

- Gremlin:

  ```
    #A10	
    auto eth0
    iface eth0 inet static
    	address 192.186.8.22
    	netmask 255.255.255.252
    
    #A11
    auto eth1
    iface eth1 inet static
    	address 192.186.12.1
    	netmask 255.255.254.0
  ```

- Thor:

  ```
    #A11
    auto eth0
    iface eth0 inet static
    	address 192.186.12.3
    	netmask 255.255.254.0
    	gateway 192.186.12.1
  ```

- Othinus:

  ```
    #A11
    auto eth0
    iface eth0 inet static
    	address 192.186.12.2
    	netmask 255.255.254.0
    	gateway 192.186.12.1
  ```

- LastOrder:

  ```
    #A7
    auto eth0 
    iface eth0 inet static
    	address 192.186.10.2
    	netmask 255.255.254.0
    
    #A8
    auto eth1
    iface eth1 inet static
    	address 192.186.9.129
    	netmask 255.255.255.128
  ```

- Leivinia:

  ```
    #A8
    auto eth0
    iface eth0 inet static
    	address 192.186.9.130
    	netmask 255.255.255.128
    	gateway 192.186.9.129
  ```

- Fuze:

  ```
    #A7
    auto eth0
    iface eth0 inet static
    	address 192.186.10.3
    	netmask 255.255.254.0
    	gateway 192.186.10.1
  ```

- Accel:

  ```
    #A3
    auto eth0
    iface eth0 inet static
        address 192.186.8.10
        netmask 255.255.255.252
    
    #A4
    auto eth1
    iface eth1 inet static
        address 192.186.9.1
        netmask 255.255.255.128
  ```

- Railgun:

  ```
    #A4
    auto eth0 
    iface eth0 inet static
    	address 192.186.9.2
    	netmask 255.255.255.128
    
    #A5
    auto eth1
    iface eth1 inet static
    	address 192.186.8.193
    	netmask 255.255.255.224
  ```

- MeltDowner:

  ```
    #A5
    auto eth0 
    iface eth0 inet static
    	address 192.186.8.195
    	netmask 255.255.255.224
    	gateway 192.186.8.193
  ```

- MentalOut:

  ```
    #A5
    auto eth0
    iface eth0 inet static
    	address 192.186.8.194
    	netmask 255.255.255.224
    	gateway 192.186.8.193
  ```

- DarkMatter:

  ```
    #A4
    auto eth0
    iface eth0 inet static
    	address 192.186.9.3
    	netmask 255.255.255.128
    	gateway 192.186.9.1
  ```

- Noukan:

  ```
    #A2
    auto eth0
    iface eth0 inet static
    	address 192.186.8.6
    	netmask 255.255.255.252
    	gateway 192.186.8.5
  ```

### Routing

Configuration to every router for routing.

- Kamachi:

  ```
    route add -net 192.186.8.4 netmask 255.255.255.252 gw 192.186.8.2   
    route add -net 192.186.9.0 netmask 255.255.255.128 gw 192.186.8.2
    route add -net 192.186.8.192 netmask 255.255.255.224 gw 192.186.8.2
    
    route add -net 192.186.8.12 netmask 255.255.255.252 gw 192.186.8.14
    route add -net 192.186.10.0 netmask 255.255.254.0 gw 192.186.8.14
    route add -net 192.186.9.128 netmask 255.255.255.128 gw 192.186.8.14
    
    route add -net 192.186.8.36 netmask 255.255.255.252 gw 192.186.8.38
    
    route add -net 192.186.8.44 netmask 255.255.255.252 gw 192.186.8.46
    route add -net 192.186.14.0 netmask 255.255.254.0 gw 192.186.8.46
    route add -net 192.186.8.224 netmask 255.255.255.224 gw 192.186.8.46
    
    route add -net 192.186.8.16 netmask 255.255.255.252 gw 192.186.8.18
    route add -net 192.186.8.20 netmask 255.255.255.252 gw 192.186.8.18
    route add -net 192.186.8.24 netmask 255.255.255.252 gw 192.186.8.18
    route add -net 192.186.12.0 netmask 255.255.254.0 gw 192.186.8.18
    route add -net 192.186.8.28 netmask 255.255.255.252 gw 192.186.8.18
    route add -net 192.186.8.32 netmask 255.255.255.252 gw 192.186.8.18
    route add -net 192.186.8.176 netmask 255.255.255.240 gw 192.186.8.18
  ```

- Fiamma:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.8.45
    route add -net 192.186.8.224 netmask 255.255.255.224 gw 192.186.14.2
  ```

- GoldenDawn:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.8.37
  ```

- Necessarius:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.8.17
    route add -net 192.186.12.0 netmask 255.255.254.0 gw 192.186.8.22
    route add -net 192.186.8.28 netmask 255.255.255.252 gw 192.186.8.26
    route add -net 192.186.8.176 netmask 255.255.255.240 gw 192.186.8.26
    route add -net 192.186.8.32 netmask 255.255.255.252 gw 192.186.8.26
  ```

- Alice:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.8.13
    route add -net 192.186.9.128 netmask 255.255.255.128 gw 192.186.10.2
  ```

- Kihara:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.8.1
    route add -net 192.186.9.0 netmask 255.255.255.128 gw 192.186.8.10
    route add -net 192.186.8.192 netmask 255.255.255.224 gw 192.186.8.10
  ```

- Vento:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.14.1
  ```

- Coronzon:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.8.25
    route add -net 192.186.8.28 netmask 255.255.255.252 gw 192.186.8.30
    route add -net 192.186.8.176 netmask 255.255.255.240 gw 192.186.8.30
  ```

- Index:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.8.29
  ```

- Gremlin:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.8.21
  ```

- LastOrder:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.10.1
  ```

- Accel:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.8.9
    route add -net 192.186.8.192 netmask 255.255.255.224 gw 192.186.9.2
  ```

- Railgun:

  ```
    route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.186.9.1
  ```

### Testing

- Client - client

  ![image](https://github.com/user-attachments/assets/6f5d4286-edbb-4bc2-9e92-a8c5f8338484)

- Client - Server

  ![image](https://github.com/user-attachments/assets/69cdce64-011c-47a4-82be-41caa1951f24)

- Client - Router

  ![image](https://github.com/user-attachments/assets/763dc4d1-8ddd-46d8-a185-b0206af9876c)

- Server - Server

  ![image](https://github.com/user-attachments/assets/11f3a143-7925-4c50-ae23-5aa17ab680ec)

- Server - Router

  ![image](https://github.com/user-attachments/assets/c533a148-71be-4003-95c4-f8107f83aab3)

- Router - Router

  ![image](https://github.com/user-attachments/assets/110238fd-6c4a-409a-a456-f4d925cd5a92)

<br>

## CIDR

### Tree

- Tree image

  `https://miro.com/app/board/uXjVLESM6V0=/?share_link_id=783363923336`
  ![image](https://github.com/user-attachments/assets/327191d2-3f68-439e-95b9-8d7d4035657d)

- IP distribution table

  ![image](https://github.com/user-attachments/assets/0c9f8967-22e1-41a9-9c04-698f88afec84)



### Subnet Merging Iteration

- Iteration 1

  ![image](https://github.com/user-attachments/assets/519c25d8-3e74-4959-87a4-baf1653b6a82)


- Iteration 2

  ![image](https://github.com/user-attachments/assets/92a692fc-410d-4c91-a90c-f836402aeff2)
  

- Iteration 3

  ![image](https://github.com/user-attachments/assets/94f766b1-04eb-43ce-a20d-572e72457aad)


- Iteration 4

  ![image](https://github.com/user-attachments/assets/5e875c48-8864-4d53-a5ec-d0057453d758)


- Iteration 5

  ![image](https://github.com/user-attachments/assets/e0018d6a-07a2-4a94-9be5-87873f969e7c)


- Iteration 6

  ![image](https://github.com/user-attachments/assets/3d908448-307f-4c7c-a410-6b0062b9d5d6)


- Iteration 7

  ![image](https://github.com/user-attachments/assets/4ce56d45-a0fe-4168-b729-1872fa67787c)


- Iteration 8

  ![image](https://github.com/user-attachments/assets/0f090ccf-0c2e-40d9-903f-67b854558d38)



### Subnetting (If you use CPT)

  `Put your subnetting configuration for each router, client, and server visualized in topology here || Masukkan konfigurasi untuk masing-masing router, client, dan server yang divisualisasikan pada topologi di sini`

### Testing

- Client - client

  `Put your testing screenshot in here`

- Client - Server

  `Put your testing screenshot in here`

- Client - Router

  `Put your testing screenshot in here`

- Server - Server

  `Put your testing screenshot in here`

- Server - Router

  `Put your testing screenshot in here`

- Router - Router

  `Put your testing screenshot in here`

<br>
  
## Problems

<br>

## Revisions (if any)

### Subnetting (If you use CPT)

  `Kamachi`
  
  ![image](https://github.com/user-attachments/assets/c2205feb-ccb8-41e5-a691-acf14aff3dd3)
  
  `Kihara`

  ![image](https://github.com/user-attachments/assets/ae472f70-a635-421c-a1b5-a0785775ede6)

  `Noukan`
  
  ![image](https://github.com/user-attachments/assets/7bae1b6c-adfa-4d5b-af72-b0ea4fc0b135)

  `Accel`

  ![image](https://github.com/user-attachments/assets/12df9538-8245-4f88-9ab2-8032cbcbd3f9)

  `DarkMatter`

  ![image](https://github.com/user-attachments/assets/43a12008-4f4b-4df8-9b92-9d94d1a93770)

  `Railgun`

  ![image](https://github.com/user-attachments/assets/536e0831-d301-41a5-9748-72e928f0dcaf)

  `MentalOut`

  ![image](https://github.com/user-attachments/assets/ad831244-464a-43e5-ad1d-6f67b13f7ba7)

  `MeltDowner`

  ![image](https://github.com/user-attachments/assets/d344968e-e92c-4723-a0c4-af2eec0d4c84)

  `Alice`

  ![image](https://github.com/user-attachments/assets/bbff6b2c-43d4-453a-a1e6-b0021bdfa231)

  `Fuze`

  ![image](https://github.com/user-attachments/assets/f7cbeaf8-2203-46ac-9c46-841ff80f9af6)

  `LastOrder`

  ![image](https://github.com/user-attachments/assets/8cae5b8e-031a-4cdd-9cfb-18d4e064050f)

  `Levinia`

  ![image](https://github.com/user-attachments/assets/3452385c-5fe3-4bfb-886d-04c97d351f15)

  `Necessarius`

  ![image](https://github.com/user-attachments/assets/03aee247-5bfe-4eef-bab1-f0a6850f6053)

  `Gremlin`

  ![image](https://github.com/user-attachments/assets/2b736273-e6bf-4e1a-b1f4-d79db6264bc5)

  `Othinus`

  ![image](https://github.com/user-attachments/assets/47ae4c8e-4c21-41c0-ae0d-edf59db2279f)

  `Thor`

  ![image](https://github.com/user-attachments/assets/72c7afc8-4444-4adf-a727-e23a4291ccd0)

  `Coronzon`

  ![image](https://github.com/user-attachments/assets/d0672243-1695-47be-a0a7-3b537c9ea7e9)

  `Index`

  ![image](https://github.com/user-attachments/assets/88241689-8d85-4475-a043-55ca8d55bf83)

  `Magnus`

  ![image](https://github.com/user-attachments/assets/5a28bae0-ee3a-4b75-983f-e3e9abfd1ced)

  `Elizard`

  ![image](https://github.com/user-attachments/assets/6931a948-3dc4-4693-a83d-91b931907515)

  `GoldenDawn`

  ![image](https://github.com/user-attachments/assets/749b41f8-25f1-4bb8-8e92-cfd17696f086)

  `Mathers`

  ![image](https://github.com/user-attachments/assets/61e8217e-c589-4c77-9400-ad85a19d3ee0)

  `Aleister`

  ![image](https://github.com/user-attachments/assets/a4bf93ee-7ed1-4a87-bd99-19047ab0402a)

  `Aiwass`

  ![image](https://github.com/user-attachments/assets/b7ad60d0-7e55-454b-84ad-cef127e60670)

  `Fiamma`

  ![image](https://github.com/user-attachments/assets/27ebccf1-32d9-48b6-a432-24afe43647cc)

  `Acqua`

  ![image](https://github.com/user-attachments/assets/baf18dba-223b-4160-bbb9-da58b2ddc48b)

  `Vento`

  ![image](https://github.com/user-attachments/assets/3246b908-faed-4ecf-a50d-bbf488bc72b9)

  `Terra`

  ![image](https://github.com/user-attachments/assets/91384d42-b162-4565-88ae-cb75545fd059)


### Testing

- Client - client

  `Aiwass-Aleister`
  
  ![image](https://github.com/user-attachments/assets/6bda951c-6d72-4fa5-a515-e50d53d5f42d)



- Client - Server

  `Thor-Othinus`
  
  ![image](https://github.com/user-attachments/assets/2ac3d989-cbcc-4821-971f-45a9cde103f7)



- Client - Router

  `Gremlin-Thor`
  
  ![image](https://github.com/user-attachments/assets/82cf0985-6fa0-468c-9d44-c216b8862a3d)



- Server - Server

  `Put your testing screenshot in here`

- Server - Router

  `Noukan-Kihara`
  
  ![image](https://github.com/user-attachments/assets/81c63717-cb7b-440f-ae5c-c688abc97e9a)


- Router - Router

  `Kamachi-Fiamma`
  
  ![image](https://github.com/user-attachments/assets/5654dc9a-cb42-4ee4-8d6d-69562f5f3f8a)



