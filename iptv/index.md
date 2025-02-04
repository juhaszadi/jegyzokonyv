
# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Juhász Ádám   
**A mérés tárgya:** Földfelszíni digitális TV vételi rendszer kiépítése, IPTV rendszer konfigurálása.    
**A mérés száma:**    
**A mérés dátuma:** 2025. 02. 03.    
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor  

--------------

## 1. Leírás

Földfelszíni digitális TV vételi rendszerének kiépítése, a jel mérésének és elosztásának elvégzése, valamint az IPTV rendszer konfigurálása.
A fogható multiplexek jelerősségének ellenőrzése, és a DVB-T jel LEMCO SCL-824CT fejállomásba történő bevezetése. A fejállomásból a digitális tartalom IPTV streamként kerül kiadásra. A Multicast IP tartomány megválasztása és az IPTV Set-top-box konfigurálása a megfelelő vételhez.



## 2. Alkalmazott mérőeszközök és készülékek

| Műszer neve                                       | 
| ------------------------------------------------- | 
| Antenna                                           | 
| LEMCO SCL-824CT 8 × DVB-S/S2/T/T2/C to 4 × DVB-T/C & IP (FTA)    |
| MAG IPTV                                          | 
| METEK HDD digitális TV jelmérő                    |
| MAG IPTV                                          |
| TP-LINK ARCHER C7 router                          |

###   Koaxiális kábelek és csatlakozók  
###   UTP kábelek
###   Jelosztó: RF16 6-os RF osztó 5-2400MHz

---------------------------------------------------------------------

## 2.1 Telepített eszközök és Felhasználási céljuk

| Telepítendő eszköz|  	Winget ID 	| Felhasználási cél| 
| ------------------|---------------|----------------- | 
| VLC 	            | VideoLAN.VLC 	| IPTV stream lejátszása és tesztelése| 
| Wireshark (TShark)| 	WiresharkFoundation.Wireshark 	| Multicast csomagok figyelése| 
| FFmpeg 	          | Gyan.FFmpeg 	| IPTV stream elemzése és rögzítése| 
| iPerf3 	          | ESnet.iPerf3 	| Hálózati teljesítménymérés| 
  
---------------------------------------------------------------------

## 3. Környezeti viszonyok, és az antenna pontos beállítása (iránytű és dőlésszög)  

1. Antenna iránya: DNY 234°    
2. Hőmérséklet: 5C°    
3. Páratartalom: 58%      
4. Légnyomás: 1027 mbar     
5. Szélsebesség: 6.8 km/h  



## 3.1 Előkészítés   

1.Internetes adatbázison elérhető multiplex a Miskolc, Avasi adótoronyból.  
(Frekvencia, teljesítmény, adás típusa) 

1.1 Használt bemenetek:    
1. multiplex A   
2. multiplex B   
3. multiplex E   
4. multiplex Miskolc TV   

Az adótorony adatbázisa elérhető itt: fmdx.hu    


<details>
    <summary>Internetes adatbázis:</summary>
   <img src="https://github.com/user-attachments/assets/4c540d76-9f1b-409f-b305-af0ef7dad8c8">
</details>

----------------------------------------------------------------

<details>
    <summary>multiplex:</summary>
   <img src="https://github.com/user-attachments/assets/6fabf81c-a03b-43a5-805f-2ca912a01042">
</details>


<details>
    <summary>multiplex:</summary>
   <img src="https://github.com/user-attachments/assets/45433386-d795-483b-ba14-992d5bd1152d">
</details>




1. Frekvencia: 634 MHz   
2. adás típusa: DVB-T    
3. jelszint: 50.3 dBuV  
4. Mer: 23.6 dB   
5. Moduláció: QPSK/8k/1/32


------------------------------------------------

## 3.2 Csatornák kiosztása

<details>
    <summary>Iniput 1: multiplex A:</summary>
   <img src="https://github.com/user-attachments/assets/91f6d06d-1985-4a3a-8479-ecfeffea774c">
</details>

Frekvencia: 666 MHz   
Channe: 45    
Bandwidth: 8MHz  

----------------------------------------------



<details>
    <summary>input 2: multipex B:</summary>
   <img src="https://github.com/user-attachments/assets/34e89440-b2ae-4fbe-8f11-17a43704c33e">
</details>

Frekvencia: 586 MHz     
Channe: 35    
Bandwidth: 8MHz     

-----------------------------------------------------


<details>
    <summary>Input 3: multiplex E:</summary>
   <img src="https://github.com/user-attachments/assets/dd8753cb-5a10-4186-82d1-e663f2126eba">
</details>

Frekvencia: 690 MHz   
Channe: 48   
Bandwidth: 8MHz    

-------------------------------------------------------


<details>
    <summary>Input 4: Miskolc TV:</summary>
   <img src="https://github.com/user-attachments/assets/9058970b-3107-420d-bbe4-a39de381f291">
</details>

Frekvencia: 634 MHz     
Channe: 41     
Bandwidth: 8MHz    


--------------------------------------------------------------


A stream UDP (User Datagram Protocol)-n keresztül jön.   

-----------------------


## 4. Hálózati tesztelés    

<details>
    <summary>Hálózati kapcsolat tesztelése multicast IP címre:</summary>
   <img src="">
</details>


<details>
    <summary>Ping teszt IPTV szerverre:</summary>
   <img src="">
</details>
  

<details>
    <summary>Traceroute vizsgálat (útvonal ellenőrzése):</summary>
   <img src="">
</details>



details>
    <summary>Wireshark csomagrögzítés IPTV stream vizsgálatához:</summary>
   <img src="">
</details>



-----------------------------------------------------------------------------------

## 4.1 IPTV stream mentése és elemzése

FFmpeg segítségével IPTV stream mentése

FFmpeg segítségével IPTV stream elemzése

FFmpeg segítségével IPTV stream csomagvesztés vizsgálata  


-------------------
## Összegzés


Készítette: Juhász Ádám  
Dátum: 2025.02.03.  







