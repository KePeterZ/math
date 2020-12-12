# Feladat
A Veni-Vidi-Vici évfolyamon mindenki kapott egy számot, és mindenki csak a másik számát tudta meg. Koszti (aki 50edik az ABC-ben) a 29-es számot kapta, P. B. Noel (aki 51edik az ABC-ben) pedig a 26-osat. A patrónusok elmondták azt is, hogy ABC sorrendben kapta meg mindenki egy számtani sorozat elemét. Koszti és Noel gondolkoznak.. Mi lehet Aletta száma? (Ő az első az ABC-ben.)

# Megoldás
```js
d = -3 // Koszti és Noel között 3 volt a különbség 1p
a[50] = a[1] + 49*d // Koszti száma 49 differencia plusz Aletta száma 2p
29 = a[1] - 147 // Átrendezzük egy kicsit 1p
a[1] = 176 // 2p

// Válasz: Aletta a 176-os számot kapta.
```