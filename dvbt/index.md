
# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Juhász Ádám   
**A mérés tárgya:** Földfelszíni digitális TV vételi rendszer telepítése, konfigurálása és mérése.    
**A mérés száma:**    
**A mérés dátuma:** 2025. 03. 10.    
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor  

--------------

## 1. Leírás

Földfelszíni digitális TV vételi rendszerének kiépítése, a jel mérésének és elosztásának elvégzése.
A megfelelő frekvencia beállítása, valamint a jelszint és egyéb paraméterek mérése. A beállított jel


## 2. Alkalmazott mérőeszközök és készülékek

| Műszer neve                                       | 
| ------------------------------------------------- | 
|INDOOR Antenna (Iskra)                             | 
| OPTICUM NYTR BOX                                  |
| MAG IPTV                                          | 
| METEK HDD digitális TV jelmérő                    |


###   Koaxiális kábelek és csatlakozók  
###   Jelosztó: RF12 6-os RF osztó 5-2400MHz

---------------------------------------------------------------------


## 2. Környezeti viszonyok, és az antenna pontos beállítása (iránytű és dőlésszög)  

1. Antenna iránya: °    
2. Hőmérséklet: 16C°    
3. Páratartalom: 59%      
4. Légnyomás: 1007 mbar     
5. Szélsebesség: 13.7 km/h

Az iskola és az adótorony közötti távolság.

<details>
    <summary>GOOGLE map:</summary>
   <img src="https://github.com/user-attachments/assets/07f635d3-2daa-442c-b126-4b8aa0e34681">
</details>



## 3.1 Előkészítés   

1.Internetes adatbázison elérhető multiplex a Miskolc, Avasi adótoronyból.  
(Frekvencia, teljesítmény, adás típusa) 

1.1 Használt bemenetek:      

1. multiplex E   (586 MHz)


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


##### Lemco SCL-824CT Programok (csatornák kiosztása)  

| #  | Input  | Program címe          | OriginalService ID | LCN  | Encrypted | TS Output | OutputService ID | IP cím      | IP port | Protokoll |
|----|--------|----------------------|-------------------|------|-----------|-----------|----------------|------------|--------|-----------|
| 1  | Input 1 | M1 HD               | 100               | 0    | FTA       | 1         | 100            | 224.0.0.2  | 10001  | UDP       |
| 2  | Input 1 | M4 Sport HD         | 101               | 0    | FTA       | 1         | 101            | 224.0.0.2  | 10002  | UDP       |
| 3  | Input 1 | Duna HD             | 102               | 0    | FTA       | 1         | 102            | 224.0.0.2  | 10003  | UDP       |
| 4  | Input 1 | DunaW/M4Sport+      | 103               | 0    | FTA       | 2         | 103            | 224.0.0.2  | 10004  | UDP       |
| 5  | Input 1 | Kossuth Radio       | 130               | 0    | FTA       | 4         | 130            | 224.0.0.2  | 10005  | UDP       |
| 6  | Input 1 | Petőfi Radio        | 131               | 0    | FTA       | 4         | 131            | 224.0.0.2  | 10006  | UDP       |
| 7  | Input 1 | Bartók Radio        | 132               | 0    | FTA       | 4         | 132            | 224.0.0.2  | 10007  | UDP       |
| 8  | Input 1 | Dankó Radio         | 133               | 0    | FTA       | 4         | 133            | 224.0.0.2  | 10008  | UDP       |
| 9  | Input 2 | M2 HD               | 200               | 0    | FTA       | 1         | 200            | 224.0.0.2  | 10009  | UDP       |
| 10 | Input 2 | M5 HD               | 201               | 0    | FTA       | 2         | 201            | 224.0.0.2  | 10010  | UDP       |
| 11 | Input 2 | TV2                 | 202               | 0    | FTA       | 1         | 202            | 224.0.0.2  | 10011  | UDP       |
| 12 | Input 2 | RTL                 | 203               | 0    | FTA       | 1         | 203            | 224.0.0.2  | 10012  | UDP       |
| 13 | Input 2 | MAX4                | 206               | 0    | FTA       | 2         | 206            | 224.0.0.2  | 10013  | UDP       |
| 14 | Input 2 | Spektrum Home +     | 207               | 0    | FTA       | 2         | 207            | 224.0.0.2  | 10014  | UDP       |
| 15 | Input 2 | MinDig TV Plusz Info | 208              | 0    | FTA       | 2         | 208            | 224.0.0.2  | 10015  | UDP       |
| 16 | Input 3 | HEVC teszt          | 524               | 0    | FTA       | 2         | 524            | 224.0.0.2  | 10016  | UDP       |
| 17 | Input 4 | Miskolc TV          | 1000              | 0    | FTA       | 2         | 1000           | 224.0.0.2  | 10017  | UDP       |


-------------------------------------------------------------------------------------------------


<details>
    <summary> VLC media playeren behozott adás statisztikája:</summary>
   <img src="https://github.com/user-attachments/assets/1af6b373-fe22-4bdd-9089-a1712fbfbc24">
</details>


------------------------------------------------------------------------------------------------

<details>
    <summary>Kodek:</summary>
   <img src="https://github.com/user-attachments/assets/aa6ff1b7-1ca4-41a1-802d-8175c51b7e01">
</details>

Puffer dimenziók: 1920x1080  
Képkocasebesség: 25
  
----------------------------------------------------------------------------------------


<details>
    <summary>Kodek2:</summary>
   <img src="https://github.com/user-attachments/assets/7e47be1f-d8aa-4446-9048-572740740e56">
</details>

Mintavételezési gyakoriság: 4800 Hz  
Bitek mintánként: 32   
Bitsebesség: 192 kb/mp  



-------------------
## Összegzés

A mérési jegyzőkönyv egy földfelszíni digitális TV vételi rendszer kiépítését és az IPTV rendszer konfigurálását dokumentálja. A mérés során a DVB-T jelet egy LEMCO SCL-824CT fejállomásba vezettem, amely a digitális tartalmat IPTV streamként továbbította. A megfelelő vétel érdekében multicast IP tartományt választottam, és konfiguráltam az IPTV Set-top-boxot. A használt eszközök között szerepelt antenna, digitális TV jelmérő, router és különböző kábelek. A router beállításai is rögzítésre kerültek, beleértve az SSID-t, jelszót és IP-címeket.

Az adás megfelelően érkezett, adatvesztés nem történt. A tesztelésből kiderült: a Mintavételezési gyakoriság (4800 Hz),  Bitek mintánként (32), Bitsebesség (192 kb/mp) A stream UDP (User Datagram Protocol)-n keresztül érkezett.
Mindezt a fentebb rögzített adatok/mérési eredmények igazolják.


---------------------------------------------------------------------


Készítette: Juhász Ádám  
Dátum: 2025.02.03.  
