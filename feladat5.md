# Feladat
Lóci egy matekórán egy trükkös kérdésen gondolkodott. Hogyan tudná a leggyorsabban összeadni az első n pozitív számot? És ha Lóci az első 200 számot szeretné összeadni? Írj neki egy könnyű egyenletet, ahol az n az első n szám amit összead!

# Válasz
```js
S[100] = N[1] + N[2] + ... + N[n] // Így kéne hosszadalmasan összeadni őket (N a lista, mert az első n pozitív számot adjuk össze) 1p
S[n] = (n/2)*(n+1) // Lócinak ez a megfelelő egyenlet 3p

// Válasz: Ha Lóci kiakarja találni n pozitív egyesével növekvő egész szám összegét, akkor az (n/2)*(n+1)-el tudja ezt megtenni.
```