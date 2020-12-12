# Feladat
```js
A robotikán Sztanó Ádám egy Legó versenyre készül. Házakat kell egymás mellé raknia, és ki kell számolnia, hogy melyikbe hány ember fér. Azt tudja, hogy egy mértani sorozattal van dolga, de még nem jött rá a szabályra. Az első ház lakosainak száma ismeretlen neki, viszont a másodikat és az ötödiket ismeri, 6 és 162. Kosztit is érdekli a feladat, ad egy csokit Ádámnak, ha megtudja mondani neki, hogy hány olyan ház van, ahol 9-nél többen laknak, viszont 1000-nél kevesebben. Segíts Ádámnak!
```

# Megoldás
```js
// Tudunk a sorozatból két elemet
a[5] = a[2]*q^3
162 = 6*q^3
q = 3 // Kitaláltuk a kvócienst 2p

a[2] = a[1]*q
6 = 3*a[1]
a[1] = 2 // Kitaláltuk a sorozat első elemét 1p

// Számoljuk ki egy egyenlőtlenséggel
15 <= 3^n <= 999 // 1p

// Ha ide elkezdjük behelyettesíteni a számokat (mert nagyon kevés van és az gyors)
// Akkor kijön, hogy 
n = [3,4,5,6] // 2p

// Válasz Koszti kérdésére: 4 olyan ház van, amiben 9nél többen, de 1000-nél kevesebben laknak.
```