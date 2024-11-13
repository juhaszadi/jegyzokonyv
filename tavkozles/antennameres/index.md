
# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Juhász Ádám 
**A mérés tárgya:** Antennák teljesítményének és jelminőségének összehasonlítása  
**A mérés száma:** 1. mérés  
**A mérés dátuma:** 2024. 11. 13  
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor  

---

## 1. Mérés célja
A mérés célja három különböző típusú antenna, az **Iskra P20**, az **ISKRA P2845** és az **IKUSI FLASHD C48** teljesítményének összehasonlítása, valamint a jelszint és jelminőség (MER - Modulation Error Ratio) vizsgálata három különböző frekvencián (474 MHz, 570 MHz, és 706 MHz).

---

## 2. Alkalmazott mérőeszközök és készülékek

| Műszer neve                         | Típus       | Gyártási szám |
| ----------------------------------- | ----------- | ------------- |
| Programozható antennaerősítő-szűrő  | Johansson   | 6700          |
| Antenna                             | Iskra       | P20, P2845    |
| Antenna                             | IKUSI       | FLASHD C48    |
| Spectrum Analizátor                 | Metek       | HDD           |

---

### 3. **Mérési helyszín és környezet**
- **Antenna magassága**: 2 m
- **Környezet jellemzői**: V3 labor
- **Adó távolsága**: 15 m

---

## 4. Antennák teljesítménye különböző frekvenciákon

| Frekvencia (MHz) | Antenna          | Jelszint (dBm) | MER (dB) | Bitsebesség (Mbps) |
| ---------------- | ---------------- | -------------- | -------- | ------------------ |
| **474 MHz**      | Iskra P20        | -61.8          | 24.6     | 8.2 – 8.6          |
|                  | ISKRA P2845      | -58.8          | 26.3     | 8.6 – 9.6          |
|                  | IKUSI FLASHD C48 | -58.5          | 27.0     | 8.4 – 9.2          |
| **570 MHz**      | Iskra P20        | -59.0          | 26.6     | 8.2 – 9.2          |
|                  | ISKRA P2845      | -52.8          | 33.2     | 8.2 – 10.0         |
|                  | IKUSI FLASHD C48 | -52.6          | 30.0     | 7.8 – 9.2          |
| **706 MHz**      | Iskra P20        | -56.0          | 24.0     | 8.4 – 9.0          |
|                  | ISKRA P2845      | -49.0          | 29.0     | 9.0 – 9.8          |
|                  | IKUSI FLASHD C48 | -49.2          | 28.4     | 8.6 – 9.4          |

---

## 5. Mérési eredmények elemzése
Az adatok alapján az alábbi következtetéseket lehet levonni:
- **Jelszint (dBm)**: Az **ISKRA P2845** és az **IKUSI FLASHD C48** antennák általában jobban teljesítettek a jelszint tekintetében, különösen a 570 MHz frekvencián. Az **ISKRA P20** antenna alacsonyabb jelszintet produkált mindhárom frekvencián.
- **MER (Modulation Error Ratio)**: A **MER** értékek alapján az **ISKRA P2845** antenna mutatta a legjobb teljesítményt, különösen a középső frekvencián (570 MHz), ahol a **MER** értéke 33.2 dB volt. Az **IKUSI FLASHD C48** antenna szintén jó **MER** értékeket ért el, de az **ISKRA P20** kicsit alulmaradt.
- **Bitsebesség**: A bitsebesség szintén magasabb volt az **ISKRA P2845** és az **IKUSI FLASHD C48** esetében, míg az **ISKRA P20** antennánál kicsit alacsonyabb értékeket tapasztaltunk. A legmagasabb bitsebességet 570 MHz-en az **ISKRA P2845** érte el (10.0 Mbps).

---

## 6. Konklúzió
Az elvégzett mérés alapján az **ISKRA P2845** antenna bizonyult a legerősebbnek mind a jelszint, mind a **MER** és bitsebesség tekintetében. Az **IKUSI FLASHD C48** szintén jól teljesített, míg az **ISKRA P20** gyengébb eredményeket mutatott. Az antennák közötti különbségek egyértelműen megmutatkoznak a különböző frekvenciákon, különösen 570 MHz-en, ahol a legnagyobb teljesítménykülönbség volt tapasztalható.

---

## 7. Mérési nehézségek és eltérések
A mérések során a labor környezetében tapasztalt esetleges zajok és interferenciák befolyásolhatták a jelszintek pontos mérését. Emellett a mérési eredmények kis mértékű eltéréseket mutathatnak az antennák pozíciójának változása miatt.

---

## 8. Grafikus ábrázolás
A jelszint és MER értékek vizuális ábrázolását az alábbi diagramok mutatják be:

![Jelszint és MER ábrázolás](https://erosbence27.github.io/jegyzokonyv/image/asd.PNG) 

---

## 9. Javaslatok
Az **ISKRA P2845** antenna javasolt elsődleges használatra, mivel minden frekvencián magasabb jelszintet és jobb jelminőséget biztosított. Amennyiben költséghatékonyabb megoldás szükséges, az **IKUSI FLASHD C48** is megfelelő választás lehet. Az **Iskra P20** csak alacsonyabb frekvenciákon javasolt, ahol még kielégítő teljesítményt nyújt.

---

## 10. P-20 Képek:
<details>
<summary>Kattins a részletekért</summary>

**474Mhz Mért Képek:**
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p20_bit474.bmp"/>
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p20_fullkep474.bmp"/>

---

**570MHz Mért Képek**
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p20_bit570.bmp"/>
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p20_fullkep570.bmp"/>

---

**706MHz Mért Képek**
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p20_bit706.bmp"/>
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p20_fullkep706.bmp"/>

---

</details>

<br>

## 11. P-2845 Képek:
<details>

<summary>Kattins a részletekért</summary>

**474Mhz Mért Képek:**
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p2845_fullkep474.bmp"/>
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p2845_bit474.bmp"/>

---

**570MHz Mért Képek**
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p2845_fullkep570.bmp"/>
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p2845_bit570.bmp"/>

---

**706MHz Mért Képek**
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p2845_fullkep706.bmp"/>
    <img src="https://erosbence27.github.io/jegyzokonyv/image/p2845_bit706.bmp"/>

---

</details>

<br>

## 12. FlashHD C-48 Képek:
<details>
<summary>Kattins a részletekért</summary>

**474Mhz Mért Képek:**
    <img src="https://erosbence27.github.io/jegyzokonyv/image/c48_fullkep474.bmp"/>
    <img src="https://erosbence27.github.io/jegyzokonyv/image/c48_bit474.bmp"/>

---

**570MHz Mért Képek**
    <img src="https://erosbence27.github.io/jegyzokonyv/image/c48_fullkep570.bmp"/>
    <img src="https://erosbence27.github.io/jegyzokonyv/image/c48_bit570.bmp"/>

---

**706MHz Mért Képek**
    <img src="https://erosbence27.github.io/jegyzokonyv/image/c48_fullkep706.bmp"/>
    <img src="https://erosbence27.github.io/jegyzokonyv/image/c48_bit706.bmp"/>

---

</details>


<br>

**Aláírás:** Erős Bence

**Dátum:** 2024. 10. 14
