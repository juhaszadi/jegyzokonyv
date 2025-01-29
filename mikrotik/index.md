# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Juhász Ádám   
**A mérés tárgya:** Komplex Távközlési Hálózat Tervezése, Telepítése és Mérése   
**A mérés száma:** 1. mérés  
**A mérés dátuma:** 2025. 01. 29.    
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor  

--------------

## 1. Alkalmazott mérőeszközök és készülékek

| Műszer neve                                       | IP. cím       | 
| ------------------------------------------------- | ----------- | 
| Mikrotik LHG18 LTE antenna                        | 192.168.188.1   |
| Mikrotik nRay 60GHz mikrohullámú antenna szett    | 192.168.88.2 és 192.168.88.3| 
| D-LINK vagy TP-LINK vagy ASUS SOHO router         | AP módban  | 


### HP switch (opcionálisan felhasználható)  
### Laptop vagy PC a konfigurációkhoz és mérésekhez  
### Iperf szoftver a sávszélesség mérésekhez   
  
---------------------------------------------------------------------

## 2. Előkészítés és tervezés

1. Eszközök gyári beállításainak visszaállítása (Factory Reset)  
   Minden eszköz gyári alaphelyzetbe állítottam  


## 2.1 Hálózati topológia

IP-cím kiosztás:

1. Mikrotik LHG18 LTE: 192.168.88.1   
2. Mikrotik nRay 60GHz Master: 192.168.88.2  
3. Mikrotik nRay 60GHz Slave: 192.168.88.3  
4. Router (AP mód): 192.168.88.4  
5. Switch (ha szükséges): 192.168.88.254  
6. Kliens laptop: 192.168.88.100-250 (DHCP-ből)  


<details>
    <summary>Topológia:</summary>
   <img src="https://github.com/user-attachments/assets/0c9e5ee7-3f29-4432-a5e5-a049cf54e7ac">
</details>


-----------------------


## 3. Hálózati tesztelés és hibakeresés  

#### Pingek a hálózaton lévő eszközökről  

Mikrotik LHG18 LTE antenna (192.168.188.1)  

Mikrotik nRay 60GHz mikrohullámú antenna szett (192.168.88.2 és 192.168.88.3)  

ASUS SOHO router (192.168.88.4)


<details>
    <summary>Tesztelés:</summary>
  C:\Users\Admin>ping 192.168.88.1

Pinging 192.168.88.1 with 32 bytes of data:
Reply from 192.168.88.1: bytes=32 time<1ms TTL=64
Reply from 192.168.88.1: bytes=32 time<1ms TTL=64
Reply from 192.168.88.1: bytes=32 time<1ms TTL=64

Ping statistics for 192.168.88.1:
    Packets: Sent = 3, Received = 3, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms
Control-C
^C
C:\Users\Admin>ping 192.168.88.2

Pinging 192.168.88.2 with 32 bytes of data:
Reply from 192.168.88.2: bytes=32 time<1ms TTL=64
Reply from 192.168.88.2: bytes=32 time<1ms TTL=64
Reply from 192.168.88.2: bytes=32 time<1ms TTL=64

Ping statistics for 192.168.88.2:
    Packets: Sent = 3, Received = 3, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms
Control-C
^C
C:\Users\Admin>ping 192.168.88.3

Pinging 192.168.88.3 with 32 bytes of data:
Reply from 192.168.88.3: bytes=32 time=1ms TTL=64
Reply from 192.168.88.3: bytes=32 time=1ms TTL=64
Reply from 192.168.88.3: bytes=32 time=1ms TTL=64
Reply from 192.168.88.3: bytes=32 time=1ms TTL=64

Ping statistics for 192.168.88.3:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 1ms, Maximum = 1ms, Average = 1ms

C:\Users\Admin>

C:\Users\Admin>ping 192.168.88.4

Pinging 192.168.88.4 with 32 bytes of data:
Reply from 192.168.88.4: bytes=32 time<1ms TTL=64
Reply from 192.168.88.4: bytes=32 time<1ms TTL=64
Reply from 192.168.88.4: bytes=32 time<1ms TTL=64
Reply from 192.168.88.4: bytes=32 time<1ms TTL=64

Ping statistics for 192.168.88.4:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds:
    Minimum = 0ms, Maximum = 0ms, Average = 0ms
   </details>

A pingek sikeresek voltak, nem történt adat vesztés.

----------

#### Tesztelés hogy elérünk-e egy külső servevrt pl.: GOOGLE (8.8.8.8)  


<details>
    <summary>Tesztelés:</summary>
   <img src="https://github.com/user-attachments/assets/46497593-8c92-4cb5-a0e1-ea7e556ada1d">
</details>


A pingek sikeresek voltak, nem történt adat vesztés. Az átlag ping értéke: 40ms



## 3.1 Sávszélesség mérése  

Az egyik laptopról (szerverként futtatjuk) ping a másikra (kliensként futtatjuk) 

<details>
    <summary>iperf:</summary>
   <img src="https://github.com/user-attachments/assets/45fd843f-31b3-48be-b69c-4a27bd5c0641">
</details>

----------

Mikrotik LHG18 LTE antenna beállításai és értékei:

|     Mikrotik LHG18 LTE antenna                    | Értékek    | 
| ------------------------------------------------- | -----------| 
| RSSI                                              | -48 dBm    |
|   RSRP                                            | -82 dBm    | 
|     SINR                                          | 18 dBm     | 
|     RSRQ                                          | -13.0 dBm  | 

A szolgáltatótól (Telekom HU) kapott IP cím: 100.88.187.247


<details>
    <summary>Mikrotik LHG18 LTE:</summary>
   <img src="https://github.com/user-attachments/assets/063adaf7-c9cd-41e0-95ce-bfe988720bfd">
</details>

-----------------

Mikrotik nRay 60GHz mikrohullámú antenna (192.168.88.3). Beállításai és jelerőssége

<details>
    <summary>Mikrotik nRay 60GHz mikrohullámú antenna:</summary>
   <img src="https://github.com/user-attachments/assets/6445fb05-179d-4b00-a68a-d2d6f7355ca7">
</details>

-------------

<details>
    <summary>Két antenna közötti átvivetli sebesség:</summary>
   <img src="https://github.com/user-attachments/assets/56232b9a-ac90-4b77-8ed1-95489e18248d">
</details>





<details>
    <summary>Speedtest:</summary>
   <img src="https://github.com/user-attachments/assets/046b4f4c-c502-4b3b-87e9-ca410f88544b">
</details>

-------------------
## Összegzés

A mérés célja egy összetett távközlési hálózat tervezése, telepítése és mérése volt.  
A hálózati topológia egy LTE kapcsolaton alapuló internetkapcsolatot, egy 60GHz-es mikrohullámú összeköttetést és egy vezeték nélküli hozzáférési pontot (AP) tartalmazott, amelyhez a kliensek csatlakoztak. A jegyzőkönyv ezen része a hálózati eszközök közötti kapcsolatok tesztelését és az esetleges hibák elhárítását tartalmazza, például ping teszteket az eszközök között.  

A jegyzőkönyv részletesen bemutatja a mérés során alkalmazott eszközöket, a hálózati topológiát és az IP-címek kiosztását, valamint a hálózati tesztelés és hibakeresés lépéseit.  

A hálózat hiba mentesen működött, adat vesztés nem történt. Össze építése és felconfigurálása nagyjából 2 órát vett igénybe.  

Készítette: Juhász Ádám  
Dátum: 2025.01.29.  







