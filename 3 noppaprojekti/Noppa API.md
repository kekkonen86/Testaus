# Noppa -luokka API


Noppa-luokka noppapelejä varten. Noppa tallettaa silmäluvun, joka voi olla välillä 
1<= silmäluku <=yläraja. Yläraja annetaan konstruktorille parametrina. Suurin sallittu yläraja on 20. Minimi yläraja on 2. Ylärajan pitää olla kokonaisluku. Jos ylärajaa ei anneta, luodaan noppa ylärajalla 6.

Jos noppaa ei ole heitetty, niin silmäluku on nolla 0. Kun noppaa on kerran heitetty, ei silmäluku voi tulla enää nollaksi.

## **Toiminnot**

### **Konstruktori**

-   alustaa nopan annetulla ylärajalla.
-   jos ylärajaa ei anneta, käytetään oletusylärajana lukua 6
-   alustaa nopan silmäluvun nollaksi 0

-   jos yläraja ei ole kokonaisluku, aiheutuu poikkeus `'Ylärajan pitää olla kokonaisluku'`
-   jos yläraja ei ole välillä 2...20, aikeutuu poikkeus:
    -   yläraja >20: `'Yläraja liian iso'`
    -   yläraja <2: `'Yläraja liian pieni'`

### **Metodit**

#### **heitaNoppaa()**
-   heittää nopan. Kun noppaa heitetään, niin silmäluvuksi tulee satunnaisluku väliltä 1...yläraja
-   ei palauta mitään

#### **toString()**
-   palauttaa nopan silmäluvun merkkijonona. Esimerkiksi `'4'`
-   jos noppaa ei ole heitetty, palauttaa merkkijonon: `'Noppaa ei ole heitetty'`

### **Getterit**

#### **pisteet**
-   palauttaa nopan silmäluvun

#### **minimi**
-   palauttaa pienimmän mahdollisen silmäluvun. Tässä 1

#### **maksimi**
-   palauttaa suurimman mahdollisen silmäluvun eli ylärajan.

