
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


## 2.1 Környezeti viszonyok, és az antenna pontos beállítása (iránytű és dőlésszög)  

1. Antenna iránya: °    
2. Hőmérséklet: 16C°    
3. Páratartalom: 59%      
4. Légnyomás: 1007 mbar     
5. Szélsebesség: 13.7 km/h

Az iskola és az adótorony közötti távolság.   

<img src="https://github.com/user-attachments/assets/07f635d3-2daa-442c-b126-4b8aa0e34681">


-------------------------------------------------------------

## 3. Előkészítés   

1.Internetes adatbázison elérhető multiplex a Miskolc, Avasi adótoronyból.  
(Frekvencia, teljesítmény, adás típusa) 

1.1 Használt bemenetek:      

1. multiplex E   (586 MHz)


Az adótorony adatbázisa elérhető itt: fmdx.hu    


<img src="https://github.com/user-attachments/assets/4c540d76-9f1b-409f-b305-af0ef7dad8c8">

----------------------------------------------------------------
## 3.2 Spektrum analizátor  

Multiplex E (586 MHz)  


<img src="https://github.com/user-attachments/assets/76cec688-310c-4d13-b891-67b77be2ba9b">


----------------------------------------

<img src="https://github.com/user-attachments/assets/f57188eb-ba2c-495b-8000-c34749912b03">

-----------------------------------------

<img src="https://github.com/user-attachments/assets/b767e702-5bb5-47f6-8ba1-a79b7ead6b11">


--------------------------------


-------------------
## Összegzés

A mérési jegyzőkönyv egy földfelszíni digitális TV vételi rendszer kiépítését és az IPTV rendszer konfigurálását dokumentálja. A mérés során a DVB-T jelet egy LEMCO SCL-824CT fejállomásba vezettem, amely a digitális tartalmat IPTV streamként továbbította. A megfelelő vétel érdekében multicast IP tartományt választottam, és konfiguráltam az IPTV Set-top-boxot. A használt eszközök között szerepelt antenna, digitális TV jelmérő, router és különböző kábelek. A router beállításai is rögzítésre kerültek, beleértve az SSID-t, jelszót és IP-címeket.

Az adás megfelelően érkezett, adatvesztés nem történt. A tesztelésből kiderült: a Mintavételezési gyakoriság (4800 Hz),  Bitek mintánként (32), Bitsebesség (192 kb/mp) A stream UDP (User Datagram Protocol)-n keresztül érkezett.
Mindezt a fentebb rögzített adatok/mérési eredmények igazolják.


---------------------------------------------------------------------


Készítette: Juhász Ádám  
Dátum: 2025.02.03.  
