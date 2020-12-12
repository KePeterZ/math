# Feladat
Az AKG-ban új épületet építenek, ahol egymás fölött van minden terem. Viszont a termek nem ugyanakkorák, hanem egyre nagyobbak. Alulról a harmadik teremben 4 ember fér el, a hetedikben pedig már 64. Mennyien férnek el a második emeleten?

# Megoldás
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