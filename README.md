# Projektek

Üdvözöllek az oldalamon ahol programozói projektjeimet tárolom!
- Minden kód szabadon letölthető és kiprobálható bármilyen észrevétel vagy hiba     esetén jelezd felém!
- Minden kódnak a leírása itt található szekciókra bontva
- English version is under construction
## Aknakereső:
- Pythonban megvalósított aknakereső játék amit konzolon lehet játszani, az alap      játékkódot megkaptam és 2 szabadon választható funckiót kellett választanom.
- Az első funkció a klasszikus zászlózó rendszert kellett megvalósitanom ami        annyit tesz, hogy amit aknának gondolunk azt lehet jelölni F X Y (F mint zászló   és X Y mint két kordináta ahova rakni szeretnénk).
-  Az UF X Y sorral peddig a zászlót tudjuk levenni ha úgy gondoljuk, hogy az        adott mezőn nincs akna
-  A másik funkció pedig egy "hint" implementáció ami felfed egy olyan mezőt ami     biztos nem akna
-  Egy játékban 3 "tipp" áll rendelkezésre.
-  A test mappában pedig a feature-ők tesztelése található
## Bejeweled:
- Javascriptben implementált Bejeweled/Candy crush játék 3 azonos színű             gyémánt egy match ami 30 pont 4-nél 40-en 5-nél 50-en.
- A játékra 120 másodperc van beállítva de ez módosítható a 17-ik sorban: ` var     idozito = 120;`(Másodpercben kell megadni az értéket)
- Gyakran előfordul, hogy nem 0 ponttal kezdődik a játék mivel még nem lett         implementálva a funckó, hogy játék elején garantáltan ne legyen match.
- A játéknak van 2 háttérzenéje is de ezt a csodás RAM-evő Chrome nem mindig        kezeli jól ezért ha valaki szeretné hallani a játék zenékit amiket mellékeltem    annak az alábbi lépések a teendők:
- Ezt a linket másold be Chrome-on belül: chrome://settings/content/sound
-  A lejátszhatnak hangot-hoz hozzáadás és a Localhost linket (amin megy a           "weboldal") kell hozzáadni és elméletben már megy is a zene.
-  Zene sorrend megcserélése lehetséges, az index.html fájlon ahol zene1 és          zene2-őt megcseréljük:
   `<audio  autoplay loop >
    <source src="EW4TH6/zene2.mp3">
    <source src="/EW4TH6/zene1.mp3">
    </audio>`
   
## ThreeJs:
- 3D modellezős projekt ahol 3D objektumokat kellett létrehozni three.js könyvtár   és Blender segítségével.
- Low poly stílus mellett döntöttem, és ementén készítettem el az autót és a        fákat Blenderben.
- A jelenetben van ambiens megvilágitás, kikapcsolható pont/reflektorfény.
- Nappal és éjjeli napszak között is lehet váltogatni.
- A szintér egérrel körbeforgatható és zoomolható.
- Van benne egy animáció, ahogy az autó az S gomb megnyomására megy körbe és        körbe, újbóli S gomnyomásra az autó megáll.
## Webshop:
- Webtervezési projekt ahol egy étteremnek az oldalát kellett megvalósítani PHP-    ban adatbázissal támogatva.
- Az oldalon lehet regisztrálni, be/kijelentkezni
- Értékelni
- Profilképet feltölteni
- Adatot módosítani
- Profilt törölni
- Kijelentkezve nem lehet rendelést leadni ha még is probálnánk a rendszer nem      fogja engedni.
- "Rendelés után" a kosár tartalma törlődik lokálisan és az adatbázisból.
  
## Az oldal beüzemelésével kapcsolatos információk PhPStorm esetén:
- Töltsük le a webshop.zip fájl és csomagoljuk ki
- Nyissuk meg a PhPStormot és egy üres projektbe, ahogy van a legfelső fő mappában    húzzunk be minden fájlt.
- Az index.php a főoldal majd ezt kell böngészőben elindítani
- Ahhoz hogy működjön az oldal kell XAMPP is ami letölthető: [XAMPP]        (https://www.apachefriends.org/hu/index.html) oldalról
- XAMPPON belül az Apache és MySQL-nél nyomjuk meg a start- gombokat
- Fontos, hogy a MySQL port egyezzen azzal ami a connect.php-ban van az alap van beállítva (3306) ha nem az akkor írjuk át arra amit alapból a XAMPP ad itt:`$PORT = 3306;`
- Utolsó lépésként pedig a zip-ben található fájlokat a XAMPP telepítési helyén belül a XAMPP/htdocs mappába is bekell húzni az összes fájlt.
