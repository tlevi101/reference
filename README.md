# Reference works

This repository collects my most important projects, from university and my other personal projects.

## Portfolio
My most recent work is my portfolio site, which I built with Laravel, Filament and Livewire, and host myself.
It is a single-page site aimed at recruiters, with an admin panel behind it.
***DISCLAIMER: It was made by Claude because i needed this fast. and i had a working version ina  few hours***

Key features:
- Multiple portfolio versions on different URLs, with Hungarian and English content.
- PDF CV generation per version and language.
- Content fully managed from a Filament admin.
- Self-made, cookieless visitor analytics: IP addresses are stored only as salted hashes, bots are filtered out.
- Light/dark theme.

Source code: [Portfolio](https://github.com/tlevi101/portfolio)
Live site: [Site](https://leventetorma.dev)

## Thesis
My other interesting project is my thesis: a multiplayer game with continuous communication between players (WebSockets).
Players must destroy the enemy with math function graphs.

Key features:
- User management: admins, players and guests.
- Live communication between players.
- Game queue.
- Map editor, custom games.
- Player friend relations.
- Math function parsing.

Source code: [Function-wars](https://github.com/tlevi101/Function-wars)

I have also deployed it, so it can be tried without cloning the project and installing every dependency: [Site](https://functionwors.leventetorma.dev/)
### ***Currently the fucntionswars websocket do not work on production, i am working on the fix. This means that cahting, and joining a game doesn't work.***
(The first login will be slow, because the backend server goes idle when there is no activity. It might take a minute or two to wake up.)

---

# Referencia munkák

Ebben a repóban gyűjtöttem össze eddigi munkáimat az egyetemről és egyéb saját projektjeimet.

## Portfólió
A legfrissebb munkám a portfólió oldalam, amit Laravel, Filament és Livewire segítségével készítettem, és magam üzemeltetek.
Egy egyoldalas, toborzóknak szánt oldal, mögötte admin felülettel.
***FONTOS: Ez Calude-al készült el, mivel gyorsan kellett egy működő verzió***

Főbb funkciók:
- Több portfólió-verzió külön URL-eken, magyar és angol tartalommal.
- PDF önéletrajz generálás verziónként és nyelvenként.
- A tartalom teljes egészében Filament adminból kezelhető.
- Saját, süti nélküli látogatottság-mérés: az IP-címek csak sózott hash-ként tárolódnak, a botokat kiszűröm.
- Világos/sötét téma.

A forráskód elérhető itt: [Portfólió](https://github.com/tlevi101/portfolio)
Élő oldal: [Oldal](https://leventetorma.dev)

## Szakdolgozat
Szakdolgozatomat külön kiemelném: egy többjátékos játékot valósítottam meg, melyben a folyamatos kommunikáció játszik nagy szerepet, ezt WebSockettel oldottam meg.
A játékosoknak matematikai függvénygrafikonokkal kell legyőzniük egymást.

Főbb funkciók:
- Felhasználókezelés: adminok, játékosok és vendégek.
- Élő kommunikáció a játékosok között.
- Játék várólista.
- Pályaszerkesztő, egyéni játékok.
- Barát kapcsolatok a játékosok között.
- Matematikai függvények értelmezése.

A forráskód elérhető ezen az oldalon: [Function-wars](https://github.com/tlevi101/Function-wars)

Továbbá kitettem egy szerverre is, így meg lehet nézni anélkül, hogy futtatni kellene lokálisan: [Oldal](https://functionwors.leventetorma.dev/)
### ***Jelenleg a websocketek nem működnek az éles szervern, dolgozoma  javításán. Ez annyit jelent, hogy chat és játékhot csatlakozás nem működik.***
(Az első belépés eltarthat egy darabig, ugyanis a backend szerver alvó állapotba kerül, ha sokáig nincs használva.)

