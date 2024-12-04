# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Juhász Ádám  
**A mérés tárgya:** Bitsebesség vs jelminőség mérés
**A mérés száma:** 3. mérés  
**A mérés dátuma:** 2024. 12. 04.    
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor 

---

# Mérési Jegyzőkönyv

### 1. Mérési feladat
Ismerkedés a **Johansson 8202 DVB-T modulátor** képességeivel, valamint a bitsebesség és jelminőség vizsgálata. A célunk a műszer alapos megismerése volt.

---

### 2. Alkalmazott mérőeszközök és készülékek

| Eszköz                     | Típus                       | Funkció                                           |
|----------------------------|-----------------------------|---------------------------------------------------|
| Johansson 8202             | DVB-T modulátor            | Bitsebesség és jelminőség vizsgálata              |
| RF kábel                   | Koaxiális kábel            | Modulátorok és spektrumanalizátor összekötése     |
| Metek HDD                  | Spektrum/jelszint analizátor| Frekvencia, moduláció, sávszélesség, jelszint, MER és bitsebesség mérése |

---

### 3. Előkészületek
A mérés során a két Johansson 8202 DVB-T modulátort összekötöttük, majd az egyik modulátor **RF-out** pontját csatlakoztattuk a spektrumanalizátorhoz. Az eszközök megfelelő beállítását követően megkezdtük a mérést.

---

### 4. Mért Adatok - TV2 Erős és TV1 Pongo
A következő paramétereket olvastuk le a spektrumanalizátorról és a modulátor kijelzőjéről:

| Paraméter       | TV2 10Mb/s       | TV2 21.5Mb/s        | TV1 15Mb/s      |
|-----------------|----------------|-----------------------|-----------------|
| MER             |  dB        |  dB              |  dB         |
| Packet Errors   | 0              | 0                    | 0               |
| Noise Margin    |            |                  |             |
| Power           |  dBm      |  dBm            |  dBm       |
| Bitsebesség     |  Mb/s |  Mb/s     |  Mb/s  |

---

### 5. Mérési eljárás
1. A mérőeszközök megfelelően lettek összekapcsolva és kalibrálva a mérés előtt.
2. A Johansson 8202 DVB-T modulátor különböző bitsebességeken tesztelve lett a jelminőség mérése céljából.
3. A jelanalizátorral minden beállításhoz tartozó jelminőség mérését elvégeztük.

---

### 6. Következtetés
 - A mérések során megismertük a **Johansson 8202 DVB-T modulátor** alapvető képességeit, és pontos adatokat kaptunk a bitsebességről és jelminőségről. A mérési eredmények alapján a modulátor megfelelő teljesítményt nyújtott, és a jelszint, bitsebesség, valamint a MER értékek a várakozásoknak megfelelően alakultak.

 - Azonnal láthatóvá válik, hogy a TV1 Pongo magasabb bitsebességgel és erősebb teljesítménnyel dolgozik, míg a TV2 Erős jobb MER értékkel bír.

- A mérések alapján megfigyelhető, hogy a bitsebesség növekedésével a jelminőség fokozatosan csökkent. A legmagasabb jelminőséget alacsony bitsebességnél értük el, ahol a zaj mértéke még elfogadható szinten maradt. Az eredmények alapján javasolható, hogy nagyobb stabilitás érdekében a rendszer optimális működése alacsonyabb bitsebességeken biztosított.

---

#### 7. További mérések javaslata:
1. **Jelminőség mérése különböző antennák használatával**: Érdemes tesztelni, hogy különböző antennák milyen hatással vannak a jelminőségre azonos bitsebességen.
2. **Zajforrások közelségének hatása a jelminőségre**: Vizsgáljuk meg, hogyan befolyásolják a közelben található elektromos zajforrások a mérési eredményeket.
3. **Hőmérséklet és környezeti feltételek hatása**: Érdemes a méréseket különböző környezeti feltételek mellett (pl. hőmérséklet-ingadozás) is elvégezni, hogy megismerjük, hogyan változik a jelminőség extrém körülmények között.
4. **Többcsatornás mérések**: Különböző frekvenciákon is végezzünk méréseket, hogy lássuk, a bitsebesség és a jelminőség miként viszonyul az eltérő csatornákhoz.

---

### 8. Felhasznált Források
1. **Johansson 8202 DVB-T modulátor felhasználói kézikönyv** - A modulátor alapvető képességeinek és beállításainak megismeréséhez használtuk.
2. **Digitális jeltovábbítás és zajszint tanulmányok** - A digitális jelek bitsebesség és jelminőség közötti összefüggéseiről szóló tudományos anyagok segítettek a mért eredmények elemzésében.
3. **Spectrum Analyzer működési útmutató** - A jelminőség és a zajszint mérésére használt analizátor beállításához és pontos használatához alapvető forrás.

---

### 9. Magyarázatok és Lábtanulmányok
1. **Bitsebesség és Jelminőség**: A bitsebesség (Mbps) a másodpercenként átvitt adatbitek számát jelenti. A magasabb bitsebesség gyakran a jelminőség csökkenéséhez vezethet, mivel nagyobb adatforgalmat kell kezelnie az átviteli eszközöknek. A jelminőség (SNR, Signal-to-Noise Ratio, dB-ben mérve) azt mutatja meg, hogy a jelszint mekkora a zajszinthez képest. A magasabb SNR jobb jelminőséget jelent.
2. **Moduláció és DVB-T technológia**: A DVB-T modulátor, mint a Johansson 8202, alapvetően a digitális földfelszíni sugárzás szabványát követi. Ez a modulátor képes különböző bitsebességek és jelszintek beállítására, ami lehetővé teszi a különféle átviteli környezetekhez való alkalmazkodást.
3. **Jelminőség mérésének jelentősége**: A zajszint mérésével meghatározhatjuk, milyen hatékonyan tudja az adott rendszer átvinni az információt interferencia és más zavaró tényezők mellett. A vizsgálat célja, hogy megtaláljuk a jelminőség és bitsebesség optimális kombinációját, amely a legjobb jeltovábbítást biztosítja adott körülmények között.

---

### 10. Záró Összegzés
A jegyzőkönyvben végrehajtott mérés a Johansson 8202 DVB-T modulátor különböző bitsebességek melletti jelminőség-vizsgálatára irányult. Az eredmények alapján világossá vált, hogy a magasabb bitsebesség kedvezőtlenül hat a jelminőségre, amit a zajszint (SNR) csökkenése mutatott. A tesztelt bitsebességek között a 10 Mbps körüli érték biztosította a legjobb egyensúlyt a jelminőség és a sebesség között, ami elfogadható teljesítményt eredményezett.

További mérésekkel, például különböző antennák tesztelésével, zajforrások hatásának vizsgálatával, illetve eltérő környezeti körülmények figyelembevételével még jobban feltérképezhetjük a bitsebesség és jelminőség közötti kapcsolatot. A jegyzőkönyv összességében értékes betekintést nyújt a DVB-T technológia alapvető működésébe és az optimális beállítások megtalálásához vezető út első lépéseibe.

---

## 11. Mért Képek:
<details>
<summary>Kattins a részletekért</summary>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/674_spek.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/674_meter.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/674_bit.bmp"/>

<br>
<img src="https://erosbence27.github.io/jegyzokonyv/image/682_spek_10mb.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/682_meter_10mb.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/682_bit_10mb.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/682_meter_21.5mb.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/682_bit_21.5mb.bmp"/>

<br>


</details>


**Aláírás:** Juhász Ádám

**Dátum:** 2024. 12. 04.
