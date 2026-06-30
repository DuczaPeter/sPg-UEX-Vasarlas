# sPg UEX Vásárlás

Egyszerűen megnyitható, egyfájlos Star Citizen commodity-beszerzési és rakodástervező.

A program a UEX API közösségi adatai alapján segít:

- több commodity együttes beszerzésének megtervezésében;
- a legalacsonyabb teljes vételár keresésében;
- készlet és konténerméret figyelembevételében;
- hajókapacitás szerinti fordulók kialakításában;
- megállók és rendszerek szerinti útvonalrendezésben;
- a pontos UEX termináltávolságok használatában, amikor azok elérhetők;
- kevesebb megállós alternatíva összehasonlításában;
- terv exportálásában és visszaimportálásában.

## Élő weboldal

A GitHub Pages bekapcsolása után az oldal ezen a címen érhető el:

**https://duczapeter.github.io/sPg-UEX-Vasarlas/**

## Aktuális verzió

**V1.0.36**

A böngészőben futó alkalmazás maga az `index.html`. Nincs szükség telepítésre, szerverre, Node.js-re vagy fordításra.

## Használat

1. Nyisd meg az élő oldalt vagy az `index.html` fájlt.
2. Jelöld ki a szükséges commodityket.
3. Add meg a kívánt mennyiségeket.
4. Válassz hajót és szükség szerint szűrőket, kiindulási helyet vagy célhelyet.
5. Kattints a **Beszerzési terv készítése** gombra.
6. Nyisd le azokat a részleteket, amelyekre szükséged van.

A commodity nevekre kattintva a hozzájuk tartozó UEX adatlap új böngészőlapon nyílik meg.

## Adatok és pontosság

Adatforrás: **UEX API 2.0**.

A UEX közösségi adatforrás. Az árak, készletek, terminálállapotok és távolsági adatok eltérhetnek a játékban ténylegesen látható állapottól. A program a rendelkezésre álló adatokból számol, és külön jelzi az ismeretlen készletet, a hiányzó távolságot vagy a tartalék útvonalsorrendet.

## Adatvédelem és helyi tárolás

- A program nem tartalmaz beégetett API-tokent.
- A beállításokat, a kiválasztásokat, az adatcache-t és a távolságcache-t a felhasználó saját böngészője tárolja.
- Ezek az adatok nem kerülnek a repositoryba és nem oszlanak meg más felhasználókkal.
- A helyi fájlként megnyitott és a GitHub Pagesen futó változat külön böngészőtárolót használ.

## Előkészített, de még nem bekötött integrációk

- sPg Ore Market
- Mission Provider

A csatlakozási pontok elő vannak készítve, de külső szolgáltató jelenleg nincs automatikusan bekötve.

## Repository szerkezete

- `index.html` – a teljes alkalmazás egyetlen fájlban
- `README.md` – dokumentáció
- `LICENSE` – MIT licenc
- `.nojekyll` – a GitHub Pages Jekyll-feldolgozásának kikapcsolása

## GitHub Pages bekapcsolása

A repositoryban:

1. Nyisd meg a **Settings** oldalt.
2. Válaszd a **Pages** menüpontot.
3. A **Build and deployment** résznél válaszd a **Deploy from a branch** lehetőséget.
4. Branch: `main`.
5. Mappa: `/ (root)`.
6. Mentsd el a beállítást.

A publikálás néhány percet vehet igénybe.

## Nem hivatalos eszköz

Ez egy nem hivatalos, közösségi Star Citizen-eszköz. Nem áll kapcsolatban a Cloud Imperium Games vállalattal. A Star Citizen és a kapcsolódó nevek a jogos tulajdonosaik védjegyei lehetnek.

## Licenc

A projekt az **MIT licenc** alatt használható.

Bárki használhatja, másolhatja, módosíthatja, terjesztheti, allicencelheti vagy értékesítheti, az MIT licenc feltételeinek megtartásával.
