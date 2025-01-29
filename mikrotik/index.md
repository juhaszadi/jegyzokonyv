# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Juhász Ádám   
**A mérés tárgya:** Komplex Távközlési Hálózat Tervezése, Telepítése és Mérése   
**A mérés száma:** 1. mérés  
**A mérés dátuma:** 2025. 01. 28.    
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


<details>
    <summary>Tesztelés:</summary>
   <img src="https://github.com/user-attachments/assets/1c4b4d46-b20e-43a2-b881-2419d9610c9d">
</details>

A pingek sikeresek voltak, nem történt adat vesztés.

----------

#### Tesztelés hogy elérünk-e egy külső servevrt pl.:GOOGLE (8.8.8.8)  


<details>
    <summary>Tesztelés:</summary>
   <img src="https://github.com/user-attachments/assets/c60249b3-8616-4243-9269-84d409408900">
</details>


A pingek sikeresek voltak, nem történt adat vesztés. Az átlag ping értéke: 28ms



## 3.1 Sávszélesség mérése  

Az egyik laptopról (szerverként futtatjuk) ping a másikra (kliensként futtatjuk) 

<details>
    <summary>iperf:</summary>
   <img src="https://github.com/user-attachments/assets/58af5248-1dc3-4e49-a04d-d8b83e73a272">
</details>

<details>
    <summary>Speedtest:</summary>
   <img src="">
</details>







