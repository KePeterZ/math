# 1. Feladat
Az AKG-ban új épületet építenek, ahol egymás fölött van minden terem. Viszont a termek nem ugyanakkorák, hanem egyre nagyobbak. Alulról a harmadik teremben 4 ember fér el, a hetedikben pedig már 64. Mennyien férnek el a második emeleten?

## Megoldás
```js
// Először kell nekünk a sorozat hányadosa. 
a[7] = a[3]*q^4
64 = 4*q^4 // 1p
q[1] = 2 // 1p
q[2] = -2 // De ez nem jó, mert mínusz ember nem lehet egy emeleten.

// Tehát q=2 esetén
a[3] = a[2]*q
4 = 2*a[2]
a[2] = 2 // 3p
// Válasz: 2.
```

# 2. Feladat
A robotikán Sztanó Ádám egy Legó versenyre készül. Házakat kell egymás mellé raknia, és ki kell számolnia, hogy melyikbe hány ember fér. Azt tudja, hogy egy mértani sorozattal van dolga, de még nem jött rá a szabályra. Az első ház lakosainak száma ismeretlen neki, viszont a másodikat és az ötödiket ismeri, 6 és 162. Kosztit is érdekli a feladat, ad egy csokit Ádámnak, ha megtudja mondani neki, hogy hány olyan ház van, ahol 9-nél többen laknak, viszont 1000-nél kevesebben. Segíts Ádámnak!

## Megoldás
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

# 3. Feladat
A Judit csibéből 5 gyerek egymás mellé rakták a telefonjukat, és észrevették, hogy a töltöttségi szintjük egy számtani sorozat. Balról az első telefon és az ötödik telefon töltöttségének összege 60 százalék volt. Az első 5 telefon együtt mennyire volt feltöltve?

## Megoldás
```js
S[5] = (a[1] + a[n])/2 * n // Használjuk a számtani megoldó képletet // 1p
S[5] = 60/2 * 5 // Behelyettesítjük a számokat // 1p
S[5] = 150 // 1p

// Válasz: Az első 5 telefon összesen 150%-ra volt töltve.
```

# 4. Feladat
A Veni-Vidi-Vici évfolyamon mindenki kapott egy számot, és mindenki csak a másik számát tudta meg. Koszti (aki 50edik az ABC-ben) a 29-es számot kapta, P. B. Noel (aki 51edik az ABC-ben) pedig a 26-osat. A patrónusok elmondták azt is, hogy ABC sorrendben kapta meg mindenki egy számtani sorozat elemét. Koszti és Noel gondolkoznak.. Mi lehet Aletta száma? (Ő az első az ABC-ben.)

## Megoldás
```js
d = -3 // Koszti és Noel között 3 volt a különbség 1p
a[50] = a[1] + 49*d // Koszti száma 49 differencia plusz Aletta száma 2p
29 = a[1] - 147 // Átrendezzük egy kicsit 1p
a[1] = 176 // 2p

// Válasz: Aletta a 176-os számot kapta.
```

# 5. Feladat
Lóci egy matekórán egy trükkös kérdésen gondolkodott. Hogyan tudná a leggyorsabban összeadni az első n pozitív számot? És ha Lóci az első 200 számot szeretné összeadni? Írj neki egy könnyű egyenletet, ahol az n az első n szám amit összead!

## Megoldás
```js
S[100] = N[1] + N[2] + ... + N[n] // Így kéne hosszadalmasan összeadni őket (N a lista, mert az első n pozitív számot adjuk össze) 1p
S[n] = (n/2)*(n+1) // Lócinak ez a megfelelő egyenlet 3p

// Válasz: Ha Lóci kiakarja találni n pozitív egyesével növekvő egész szám összegét, akkor az (n/2)*(n+1)-el tudja ezt megtenni.
```