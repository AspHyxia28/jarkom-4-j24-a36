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

  `Server (Noukan, MentalOut, Mathers, Othinus, Elizard)`
  ![image](https://github.com/user-attachments/assets/e54dbbe5-fc4a-4bee-b851-13bc00acb732)
  ![image](https://github.com/user-attachments/assets/b0017fa0-34da-4362-bd4c-cd6bb4401454)
  ![image](https://github.com/user-attachments/assets/69d78788-623e-4ea0-8319-f4eae6739daf)
  ![image](https://github.com/user-attachments/assets/9f6693aa-b8d4-493c-add4-060d09216630)
  ![image](https://github.com/user-attachments/assets/30129820-bca6-4db9-b106-11eb850b8200)

  `PC (DarkMatter, Terra, Acqua, Aiwass, Fuze, Aleister, MeltDowner, Lavinia, Thor, Magnus)`
  ![image](https://github.com/user-attachments/assets/ea09a645-91b8-42aa-8a7e-9a8552206b02)
  ![image](https://github.com/user-attachments/assets/30a46f35-5092-40b8-919b-30864a867a01)
  ![image](https://github.com/user-attachments/assets/ac25b349-a8fe-418f-9111-fd523d884835)
  ![image](https://github.com/user-attachments/assets/605e6644-002b-4f44-bfd6-78fcd29c7626)
  ![image](https://github.com/user-attachments/assets/6f6b6993-bcc6-4347-8ed7-16019e47ae84)
  ![image](https://github.com/user-attachments/assets/066ab495-11be-43d8-8b31-bb51be628019)
  ![image](https://github.com/user-attachments/assets/8c9082c9-caa4-4806-82d7-0db1e5738244)
  ![image](https://github.com/user-attachments/assets/bb3d7377-83a3-49cf-be51-e7a4de9a4a1a)
  ![image](https://github.com/user-attachments/assets/cc486fdb-0175-4da2-ae38-bea99db9675d)
  ![image](https://github.com/user-attachments/assets/071ae5c1-207e-4b40-b58b-82a7d184c757)

  (Config router dapat dilihat dari pkt yang diberikan)


### Testing

- Client - client

  `Aiwass-Aleister`
  ![image](https://github.com/user-attachments/assets/437b562a-51db-4747-bedd-0febb6cb598e)


- Client - Server

  `Thor-Othinus`
  ![image](https://github.com/user-attachments/assets/9175b949-4f1b-4ae1-9790-66d627a66ca8)


- Client - Router

  `Gremlin-Thor`
  ![image](https://github.com/user-attachments/assets/b55b7d3c-2552-40c0-b33a-74b83e3c2533)


- Server - Server

  `Put your testing screenshot in here`

- Server - Router

  `Noukan-Kihara`
  ![image](https://github.com/user-attachments/assets/4064ffaf-a825-44ca-980f-0abe402bac01)


- Router - Router

  `Kihara-Kamachi`
  ![image](https://github.com/user-attachments/assets/e2258332-7a32-42e8-8a52-5dd811d70ae5)


