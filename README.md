# Tesztautomatizálási kérdések

## Tesztelési alapok (ISTQB-hez kapcsolódó)
<img src="https://www.mindsmapped.com/wp-content/uploads/2016/06/ISTQB.jpg" alt="image" width="300" height="220">

#### ✅ Mi a tesztelés célja? Mi nem az?
Célja:

A hibák feltárása és javítása a fejlesztési folyamatban. Annak biztosítása, hogy a szoftver megfeleljen a specifikációknak és az ügyfél elvárásainak. A termék minőségének és megbízhatóságának növelése. Kockázatok csökkentése a szoftver használata során. Nem célja:

Az összes hiba megtalálása (ez szinte lehetetlen). A hibamentesség garantálása. Kizárólag a hibakeresés, mivel a tesztelés a megelőzés és a minőség biztosítása is.


#### ✅ Mik a tesztelési alapelvek?
Hibák jelenlétének bizonyítása: A tesztelés célja hibák feltárása, nem azok hiányának bizonyítása. Kimerítő tesztelés nem lehetséges: Lehetetlen minden kombinációt tesztelni; prioritást kell adni a kritikus területeknek. Korai tesztelés: A tesztelést már a fejlesztési ciklus elején el kell kezdeni. Hibahalmozódás: A hibák gyakran egy adott területen koncentrálódnak. A parkinsoni tesztelés: A tesztelés csak az elérhető erőforrásokhoz igazodva történik. Tesztelés a kontextustól függ: Más-más tesztelési megközelítések szükségesek például egy webalkalmazás és egy beágyazott rendszer esetén. A hibák hiánya téveszme: Egy hibamentes szoftver is lehet használhatatlan, ha nem felel meg az üzleti követelményeknek.


#### ✅ Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?
Az egységtesztelés a szoftver legkisebb önálló komponensének (pl. egy függvény vagy osztály) tesztelése, hogy az megfelelően működjön.

Felelős: Általában a fejlesztők írják az egységteszteket, mivel ők ismerik legjobban a kódot és annak működését.


#### ✅ Mik a tesztszintek, és mi a különbség köztük?
Egységtesztelés: Az egyes komponensek tesztelése különállóan. Integrációs tesztelés: A modulok vagy komponensek közötti interakció tesztelése. Rendszertesztelés: A teljes rendszer működésének tesztelése. Elfogadási tesztelés (UAT): Annak biztosítása, hogy a rendszer megfelel az ügyfél elvárásainak. Különbség: A szintek a rendszer különböző rétegeit célozzák, az egységtől (legalacsonyabb szint) az egész rendszeren át (legmagasabb szint).


#### ✅ Mi a különbség a verifikáció és a validáció között?
Verifikáció (ellenőrzés): Annak vizsgálata, hogy a szoftver fejlesztése a specifikációk szerint történik-e. („Jól csináljuk-e a dolgokat?”) Példa: Kód review, statikus tesztelés. Validáció (érvényesítés): Annak biztosítása, hogy a szoftver megfelel az ügyfél igényeinek. („A jó dolgot csináljuk-e?”) Példa: Felhasználói tesztelés, dinamikus tesztelés.


#### ✅ Mik a tesztelési típusok, és mi a különbség köztük?
Funkcionális tesztelés: Ellenőrzi, hogy a szoftver megfelel-e a funkcionális követelményeknek. Nem-funkcionális tesztelés: Teljesítmény, biztonság, használhatóság, stb. vizsgálata. Regressziós tesztelés: Annak biztosítása, hogy egy új módosítás nem okozott hibát a korábban működő funkciókban. Exploratory (feltáró) tesztelés: A tesztelő kreatív szabadságot kap a hibák keresésére. Különbség: A típusok a vizsgálat fókuszában és a módszerekben térnek el.


#### ✅ Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?
Fehér doboz: A tesztelő ismeri a kódot és a belső működést. Példa: Kódlefedettségi teszt. Fekete doboz: A tesztelő nem ismeri a belső működést; csak a bemeneteket és kimeneteket vizsgálja. Példa: Funkcionális tesztelés. Szürke doboz: Részleges ismerettel rendelkezik a rendszer működéséről, és mindkét megközelítést kombinálja.


#### ✅ Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?
UAT: Az ügyfél vagy végfelhasználó végzi, hogy ellenőrizze a rendszer megfelelőségét az üzleti igényekhez. Rendszerteszt: A teljes rendszer funkcióinak és nem-funkcionális aspektusainak tesztelése a fejlesztők vagy tesztelők által. Különbség: Az UAT az üzleti elvárásokra, míg a rendszerteszt a műszaki megfelelésre összpontosít.


#### ✅ Sorolj fel különbségeket a regressziós tesztelés, a füsttesztelés és az újratesztelés között!
Különbségek: Regressziós tesztelés, füsttesztelés és újratesztelés Regressziós tesztelés: Annak biztosítása, hogy a meglévő funkciók nem sérültek új módosítások miatt. Füsttesztelés: Az alapvető funkciók gyors ellenőrzése, hogy a rendszer egyáltalán működik-e. Újratesztelés: Egy konkrét hiba javításának ellenőrzése. Különbség: A regresszió szélesebb körű, a füstteszt gyors és alapvető, az újratesztelés pedig célzott.


#### ✅ Mi a különbség a statikus és dinamikus tesztelés között?
Mi a különbség a statikus és dinamikus tesztelés között? Statikus tesztelés: A kód és dokumentáció átnézése futtatás nélkül (pl. kód review). Dinamikus tesztelés: A szoftver futtatása közbeni tesztelés (pl. funkcionális tesztelés). Különbség: A statikus tesztelés nem igényli a kód futtatását, míg a dinamikus igen.


### ✅ Hasonlítsd össze a V-modellt, a vízesés modellt és az Agile megközelítést a tesztelés szempontjából!
Modell	Fő jellemző	Tesztelési megközelítés V-modell	Fázisokra bontott, szigorúan kötött	A tesztelés minden fejlesztési fázissal párhuzamosan történik (verifikáció és validáció). Vízesés	Lineáris, egymásra épülő fázisok	A tesztelés késői szakaszban kezdődik (főleg rendszerteszt és elfogadási teszt). Agile	Iteratív és rugalmas	A tesztelés folyamatosan történik minden sprintben, nagy hangsúly van az automatizáláson.



<img src="https://t4.ftcdn.net/jpg/03/90/15/65/360_F_390156585_8w1lsOyICIAOvDCU8tExXW2QwLCOFwXD.jpg" alt="image" width="550" height="400">


<img src="https://i.imgur.com/S38EBJw.png" alt="image" width="550" height="400">   <img src="https://segedletek.level14.hu/assets/img/modszertan-vizeses.svg" alt="image" width="550" height="400">


<img src="https://promanconsulting.hu/wp-content/uploads/2022/03/agilis-modszertanok-optimized.jpg" width="550" height="400">





## Reporting, Bugs
<img src="https://moolya.com/blog/wp-content/uploads/2023/05/Bug-Report.png" alt="image" width="300" height="220">

#### ✅ Milyen lépéseket követnél egy hiba megtalálásakor?
- A hiba észlelése / gyanúja
Valamilyen viselkedés eltér a vártól – ez lehet UI-hiba, funkcionális probléma, összeomlás stb.

- Reprodukciós környezet előkészítése
Ellenőrzöm, milyen környezetben történt a hiba (pl. böngésző, OS, verzió, build). Ugyanabban a környezetben próbálom meg reprodukálni.

- Reprodukció lépésről lépésre
Tudatosan végigjárom a hiba felé vezető utat: pontos inputok, kattintások, állapotok. Ha reprodukálható, az már értékes információ.

- Logok és technikai információk gyűjtése

- Konzol log, hibakód, stack trace, HTTP válaszok stb.

- Képernyőmentés vagy videó készítése a hibáról.

- Hiba izolálása
- Megnézem, hogy más környezetben, más verzióval vagy más felhasználói - szerepkörrel is jelentkezik-e. Ha nem, az is kulcsfontosságú információ.

- Hibajelentés készítése (részletek lentebb)

- Kommunikáció a fejlesztőkkel / csapattal
- Kérdés esetén egyeztetek, pontosítok, visszajelzést adok, ha a hiba státusza változik.

#### ✅ Beszélj a gyakori tesztjelentésekről és részleteikről!
- A leggyakoribb tesztjelentések:

 - Hibajelentés (Bug Report)
    - Olyan jelentés, amely dokumentálja, ha a szoftver nem a specifikáció szerint viselkedik.

- Tesztelési státuszjelentés (Test Execution Report)
    - Egy adott sprint vagy build során lefuttatott tesztek eredményei:

    - Hány teszt sikeres / sikertelen / kihagyott

    - Lefedettség, státuszok, tendenciák

- Hibatérkép (Bug Summary Report)
    - Grafikonos összesítés a hibák állapotáról, súlyosság szerint bontva. Például:

    - 10 Critical

    - 5 Major

    - 12 Minor
    - Ezekből következtethetünk a termék érettségére.

- Teszteset dokumentáció / test case leírás
Minden egyes teszt részletes leírása:

    - Cél

    - Lépések

    - Bemenet / elvárt kimenet

    - Teszt státusza


#### ✅ Mit tartalmaz egy hibajelentés?
Egy jó hibajelentés egyértelmű, reprodukálható és részletes. Tartalma:

- Cím (Title)
    - Rövid, de informatív, pl.:
    - „[BUG] A ‘Mentés’ gomb nem működik Firefox alatt (v1.2.3)”

- Környezeti információk
    - OS, böngésző, alkalmazásverzió, eszköz típusa stb.

- Reprodukálás lépései

    - Belépés admin felhasználóként

    - Navigálás a Beállítások → Mentés fülre

    - Kattintás a „Mentés” gombra

- Elvárt eredmény
    - A változások mentődnek és visszajelzés jelenik meg.

- Tényleges eredmény
    - Gomb nem reagál, a változások elvesznek.

- Log, hibaüzenet, stack trace (ha van)
    - Konzol: Uncaught TypeError: Cannot read property 'save' of undefined

- Képernyőkép / videó (nagyon hasznos)

- Súlyosság (Severity)
    - Pl.: Blocker, Critical, Major, Minor

- Prioritás (Priority)
    - Business szempontból mennyire fontos.

#### ✅ Hogyan rangsorolnál egy hibát?
A hibák rangsorolása két tengely mentén történik:

➤ Severity (Súlyosság) – technikai hatás
Blocker – Nem lehet belépni, rendszer összeomlik

- Critical – Fő funkció nem működik (pl. nem lehet vásárolni)

- Major – Komoly funkciós hiba, de van kerülőút

- Minor – UI hiba, helyesírás, kis kényelmetlenség

- Trivial – Alig észrevehető, esztétikai jellegű

➤ Priority (Prioritás) – üzleti hatás
- P1 – Azonnali javítás szükséges

- P2 – Következő sprintben javítandó

- P3 – Alacsony prioritás, ráér

- P4 – Nem sürgős, backlogba mehet

- Egy hiba lehet Critical-Magyarul P3, ha például csak nagyon ritka esetben jön elő, de technikailag súlyos.


## Test Automation, Selenium
<img src="https://media.licdn.com/dms/image/C4D12AQE3GOyVsZazOw/article-cover_image-shrink_600_2000/0/1583830696602?e=2147483647&v=beta&t=bYHbKyhMoWsMgtEug6eSf3m0db5ZtGEl437TeS1qkfI" alt="image" width="320" height="220">

#### ✅ Melyik teszteseteket érdemes automatizálni és melyiket nem?
- Érdemes automatizálni:

    - Gyakran ismétlődő tesztek (pl. regressziós tesztek)

    - Stabil, kevéssé változó funkciók (pl. bejelentkezés, űrlap beküldés)

    - Több böngészőben / környezetben is tesztelendő funkciók

    - Adatvezérelt tesztek – sokféle bemenettel ugyanaz a teszt

    - Teljesítménytesztek (load, stressz)

    - Füsttesztek (smoke tests) – alaprendszer működik-e

- Nem érdemes automatizálni:

    - Gyakran változó felületek / dizájn elemek

    - Komplex vizuális ellenőrzések (pl. UI kinézete)

    - Egyszeri tesztesetek vagy gyors manuális ellenőrzések

    - Feltáró tesztelés (exploratory testing)
#### ✅ Írj le egy jó automatizált tesztet!
- Egyértelmű, célorientált

- Használható többféle inputtal (adatvezérelt módon)

- Stabilan teszteli a fő funkciót

- Hibajelzés esetén pontosan mutatja, hol a probléma



#### ✅ Mi a Selenium, Selenium IDE és Selenium WebDriver?

- Selenium: Nyílt forráskódú tesztelési keretrendszer webalkalmazásokhoz.

- Selenium IDE:

    - Böngésző bővítmény (Chrome/Firefox)

    - Legegyszerűbb mód tesztek felvételére (record & playback)

    - Nem túl rugalmas, inkább tanulásra és gyors demókra jó

- Selenium WebDriver:

    - Programozható interfész Python, Java, C#, JS stb. nyelveken

    - Közvetlenül vezérli a böngészőt

    - Rugalmas, ipari szintű automatizálásra való

#### ✅ Hogyan lehet azonosítani a webes elemeket?
Webes elemek azonosítása a DOM alapján:

- By.id("...")

- By.name("...")

- By.class_name("...")

- By.tag_name("...")

- By.link_text("...")

- By.partial_link_text("...")

- By.css_selector("...") – erőteljes, rugalmas

- By.xpath("...") – nagyon pontos, akár a DOM-szerkezet szerint

#### ✅ Hogyan lehet várni az elemekre, és mi lehet a probléma? Gyűjtsd össze a lehetséges hibákat és okokat!
- Implicit wait:
Egyszer beállítva minden elemre vár a megadott ideig
Pl.: driver.implicitly_wait(10)
- Explicit wait:
Adott elemre várunk adott feltétellel
- Fluent wait:
Több beállítás (pl. polling idő, kivételek figyelmen kívül hagyása)
Gyakori problémák és okok:
Az elem még nem látható / nem kattintható
AJAX vagy JavaScript lassan tölti be
Oldal frissül közben → elem eltűnik
Nem megfelelő az azonosító (pl. dinamikus ID)


#### ✅ Hasonlítsd össze a POM és a Keyword Driven Testing megközelítéseket!
A Page Object Model (POM) egy olyan tervezési minta, ahol minden egyes weboldalhoz vagy felhasználói felülethez létrehozunk egy külön osztályt vagy objektumot. Ezek az osztályok tartalmazzák az oldal elemeit és a velük végezhető műveleteket. Például lehet egy LoginPage nevű osztály, ami tudja, hogyan kell beírni a felhasználónevet, a jelszót, és hogyan kell rákattintani a belépés gombra. Ez a megközelítés erősen kódalapú, és elsősorban fejlesztők vagy automatizálási mérnökök használják.
Ezzel szemben a Keyword Driven Testing módszernél előre definiált kulcsszavakat használunk a tesztek összeállításához. Ezek a kulcsszavak például lehetnek olyan műveletek, mint „Login”, „Click”, „Enter Text”, stb. A tesztesetek gyakran Excel vagy más táblázatos formában készülnek, ahol a tesztelők az előre megadott kulcsszavakat és a hozzájuk tartozó adatokat adják meg. Ez a módszer lehetővé teszi, hogy még programozási tudás nélkül is lehessen automatizált tesztet készíteni.
Összefoglalva:
A POM jobban alkalmas nagyobb, strukturált automatizálási projektekhez, ahol újrafelhasználható kódra van szükség,
míg a Keyword Driven Testing inkább akkor hasznos, ha a teszterek nem fejlesztők, és a teszteket inkább üzleti szempontból, táblázatos módon szeretnék kezelni.


#### ✅ Mi a különbség a TDD és BDD között?
A TDD, vagyis a tesztvezérelt fejlesztés azt jelenti, hogy a fejlesztő először megírja a teszteket egy funkcióhoz, még mielőtt maga a funkció elkészülne. Ezek általában egységtesztek, amelyek kód szinten, kis komponenseket ellenőriznek. A fejlesztő addig dolgozik a funkción, amíg az összes teszt át nem megy. Ez nagyon technikai megközelítés, és főként a fejlesztői csapat használja.
A BDD, vagyis a viselkedés-vezérelt fejlesztés inkább üzleti szemléletű. Itt a tesztek a szoftver elvárt viselkedését írják le egy mindenki számára érthető formában. Gyakran használnak „Given – When – Then” (Adott – Amikor – Akkor) formátumot, amelyet például a Gherkin nyelven írnak le. Ebben nemcsak fejlesztők, hanem üzleti elemzők és tesztelők is részt vesznek, így a kommunikáció is hatékonyabb.
Összefoglalva:
A TDD technikai szemléletű és kódszintű automatizálásra koncentrál,
míg a BDD célja a viselkedés leírása, és az üzleti és fejlesztői igények összehangolása.

#### ✅ Mi az API tesztelés és miért hasznos?

API tesztelés:
Webszolgáltatások és REST API-k működésének ellenőrzése.
Előnyei:
Gyors – nincs UI, közvetlenül hívjuk az endpointokat
Stabil – UI változás nem befolyásolja
Korai hibafogás – már backend szinten észlelhetjük
Adatellenőrzés – JSON válasz, státuszkód, fejlécek, teljesítmény
Példa eszközök:
Postman
REST Assured (Java)
pytest + requests (Python)
SoapUI

#### ✅ Mi az adatvezérelt tesztelés és miért hasznos?
Data-Driven Testing (DDT):
A tesztelés során külön adatforrásból (CSV, Excel, JSON, DB) töltjük be a bemeneti értékeket.
Miért hasznos?
Ugyanazt a tesztlogikát többféle adattal tudjuk lefuttatni
Könnyebb karbantartás: tesztkód ≠ tesztadat
Nagyobb lefedettség, kevesebb kód