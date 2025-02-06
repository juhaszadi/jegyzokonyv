# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Juhász Ádám   
**A mérés tárgya:**  Vezeték nélküli hálózat kiépítése    
**A mérés száma:**   
**A mérés dátuma:** 2025. 02. 06.    
**A mérést vezette:** Csontos Dénes  

**Évfolyam:** 13. E  
**Csoport:** GYAK 1  
**Helyszín:** Fizikai Labor  

--------------

## 1. Alkalmazott mérőeszközök és készülékek

| Műszer neve                                       | IP. cím       | 
| ------------------------------------------------- | ----------- | 
|           Catalyst 2950 switch                    |              |
|  Tenda router                                     |  192.168.3.254 | 
|      ThinkPad laptop                              | DHCP | 
|      Mobiltelefon                                 |  |


1.Catalyst 2950 switch: Hálózati eszközök közötti kapcsolatot biztosította.   
2.Tenda: Hálózat központi irányítószerv.   
3.ThinkPad laptop: A teszteléshez, ping tesztek és egyéb parancsok.  
4.Mobiltelefon: Linksys routerhez, hogy a laptop és a többi eszköz között pingelni lehetsen.
 
  
---------------------------------------------------------------------

## 2. Előkészítés és tervezés

1. Eszközök gyári beállításainak visszaállítása (Factory Reset)  
   Minden eszköz gyári alaphelyzetbe állítottam  


## 2.1 Hálózati topológia

A hálózati topológia Cisco Packet Tracer-ben lett megtervezve.   


IP-cím kiosztás:

1.Catalyst 2950 switch:    
2.Tenda router:   
3.ThinkPad laptop: 
4.Mobiltelefon: 
 


<details>
    <summary>Topológia:</summary>
   <img src="https://github.com/user-attachments/assets/9df26b29-6c85-4255-bce0-2098f346c374">
</details>


-----------------------

## 3. A számítógép IP beállításai     

## 3.1 Az aktuális IP-cím eldobása   
Parancs: `ipconfig /release`    

<details>
    <summary>Topológia:</summary>
   <img src="">
</details>



## 3.2 Új IP-cím kérése   
Parancs: `ipconfig /renew`   

<details>
    <summary>Topológia:</summary>
   <img src="">
</details>


## 3.3 A routing tábla megjelenítése   
Parancs: `netstat -a`


<details>
    <summary>Topológia:</summary>
   <img src="">
</details>


------------------------------------------------------------------

## 4. Hálózat tesztelése  

## 4.1 A microsoft.com szerver elérhetőségének tesztelése   


<details>
    <summary></summary>
   <img src="">
</details>


## 4.2 Az www.ipon.hu szerver felé vezető útvonal lekövetése  

<details>
    <summary>:</summary>
   <img src="">
</details>


## 4.3 Használt portok listázása    


<details>
    <summary>:</summary>
   <img src="">
</details>

## 4.4 Hálózati kapcsolatok megjelenítése    


<details>
    <summary>:</summary>
   <img src="">
</details>


## 4.5 DNS-beállítások aktualizálása       

<details>
    <summary>:</summary>
   <img src="">
</details>



## 4.6 Csatolt hálózati meghajtók megjelenítése     

<details>
    <summary>:</summary>
   <img src="">
</details>





## 4.7 A www.ipon.hu tartománynév és IP-cím megjelenítése  


<details>
    <summary>:</summary>
   <img src="">
</details>




---------------------------------------------------------------------------------

## 5. Telefonos tesztelés   


## 5.1 Telefon rákapcsolódva a Wi-Fi-re  

<details>
    <summary>:</summary>
   <img src="">
</details>



## 5.2 Telefon pingelése laptopról  

<details>
    <summary>:</summary>
   <img src="">
</details>



----------------------------------------------------
## 6. Router konfigurációk


-------------------
## Összegzés

Szar az egesz, atirtam a router ip cimet 192.163.3.254 es nem volt utana netem sehol se. :DDDD


Készítette: Juhász Ádám  
Dátum: 2025.02.06.  
