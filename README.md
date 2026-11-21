# AutoPark – telepítési útmutató

Az AutoPark Android-alkalmazás, amely az autóban töltött utakat naplózza, és segít a parkolás
SMS-es indításában és leállításában. Ebben a repóban csak a **kész telepítőfájlok (APK-k)** vannak,
a [Releases](https://github.com/mignac2/autopark/releases) oldalon.

> Az app nincs a Google Play áruházban. Ezért a telepítés kicsit más, mint megszokott: egyszer engedélyezni kell
> az „ismeretlen forrásból” való telepítést. Ezután a frissítéseket maga az app ajánlja fel.

## Követelmények

- Android 10 vagy újabb telefon
- kb. 120 MB szabad hely

## Első telepítés

1. Nyisd meg a telefonon ezt az oldalt:
   **https://github.com/mignac2/autopark/releases/latest**
2. Az *Assets* részben koppints az `autopark-<verzió>.apk` fájlra. A letöltés elindul (kb. 50 MB, érdemes wifin).
   - Ha a Chrome figyelmeztet, hogy a fájl „ártalmas lehet”, válaszd a **Letöltés mindenképp** lehetőséget.
3. Ha kész, koppints a letöltött fájlra (az értesítésben vagy a *Fájlok* / *Letöltések* alkalmazásban).
4. Az Android először valószínűleg ezt írja: *„Biztonsági okokból a telefon nem telepíthet ismeretlen
   alkalmazásokat ebből a forrásból.”*
   - Koppints a **Beállítások** gombra.
   - Kapcsold be: **Engedélyezés ebből a forrásból**.
   - Lépj vissza.
5. Koppints a **Telepítés** gombra.
6. Ha a Google Play Protect rákérdez, válaszd a **Telepítés mindenképp** lehetőséget (vagy *Részletek* →
   *Telepítés mindenképp*). Ez azért van, mert az app nem a Play áruházból jön.
7. Nyisd meg az AutoParkot, és add meg a kért engedélyeket.

## Frissítés

Nem kell ezt az oldalt figyelned:

- Az app naponta egyszer megnézi, hogy van-e új verzió. Ha van, egy **„Új AutoPark verzió: …”** értesítést kapsz
  (ez csak a telefonon jelenik meg, az órán nem).
- Koppints az értesítésre, majd a **Letöltés és telepítés** gombra.
- Az első alkalommal az Android kérheti, hogy engedélyezd az AutoParknak az alkalmazástelepítést
  (*ismeretlen források*). Az app odavisz a megfelelő beállításhoz: kapcsold be, majd lépj vissza.
- Az app letölti az új verziót, ellenőrzi (ellenőrzőösszeggel), majd az Android megkérdezi, telepítse-e:
  koppints a **Frissítés** gombra.
- A beállításaid és a naplód megmaradnak.

**Kötelező frissítés** feliratot akkor látsz, ha a régi verzió már nem működik megbízhatóan. Ilyenkor
frissíts, amint lehet.

Ha valamiért kézzel frissítenél: töltsd le az új APK-t a fenti linkről, és telepítsd ugyanúgy, mint elsőre.
A meglévő app fölé települ, nem kell előbb eltávolítani.

## Gyakori problémák

- **„Az alkalmazás nincs telepítve” / „ütközik egy meglévő csomaggal”**: van a telefonon egy másik
  (pl. fejlesztői/teszt) AutoPark, amelyet más kulccsal írtak alá. Ilyenkor azt előbb el kell távolítani
  (ezzel a naplója is törlődik), utána települ az új.
- **Nem jön frissítési értesítés**: nézd meg, hogy az AutoPark értesítései engedélyezve vannak-e
  (Beállítások → Alkalmazások → AutoPark → Értesítések → „Frissítések”).
- **A letöltés megszakadt**: koppints újra az értesítésre vagy a **Letöltés és telepítés** gombra.

## Biztonság

Minden kiadást ugyanaz a kulcs ír alá. Az Android csak akkor engedi a frissítést, ha az új verzió is ezzel
a kulccsal készült. A tanúsítvány SHA-256 ujjlenyomata:

```
59:F3:58:6C:61:0F:A4:E7:EE:D6:68:EC:DE:3F:1C:DF:66:12:0C:CA:69:10:34:18:3F:7D:3B:68:CB:25:6C:BD
```
