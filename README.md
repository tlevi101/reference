# Reference works

This repository collects my most important projects, from university and my other personal projects.

## Portfolio
My most recent work is my portfolio site, which I built with Laravel, Filament and Livewire, and host myself.
It is a single-page site aimed at recruiters, with an admin panel behind it.

***DISCLAIMER: It was made by Claude because i needed it asap.***

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
To try the game you may enter as a guest, however you must enter from 2 different browsers with 2 different guest. 

Key features:
- User management: admins, players and guests.
- Live communication between players.
- Game queue.
- Map editor, custom games.
- Player friend relations.
- Math function parsing.

Source code: [Function-wars](https://github.com/tlevi101/Function-wars)

I have also deployed it, so it can be tried without cloning the project and installing every dependency: [Site](https://functionwors.leventetorma.dev/)
### <del> ***Currently the fucntionswars websocket do not work on production, i am working on the fix. This means that cahting, and joining a game doesn't work.*** </del> FIXED: Cloudflare blocked websockets.

## Java Snake game

It’s a small generic snake game.

### [Source Code](https://github.com/tlevi101/snake-java)

## C#/WPF Snake game

Implements the same features as the Java version.

### [Source Code](https://github.com/tlevi101/snake-cs)

## PC monitoring webserver (C#)

It’s a small personal project that I abandoned. It was meant to be combined with Wallpaper Engine, which is a Windows app used to display HTML, videos, and small apps as a wallpaper. I made a custom modification to my PC by adding a screen to the side of my PC case and making it semi-transparent while displaying information on the screen.
---

# Referencia munkák
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

[Forráskód](https://github.com/tlevi101/portfolio)
[Oldal](https://leventetorma.dev)

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
### <del> ***Jelenleg a websocketek nem működnek az éles szervern, dolgozoma  javításán. Ez annyit jelent, hogy chat és játékhot csatlakozás nem működik.*** </del> Javítva: Cloudflare blokolta Websocket kapcsolatokat

## Java Kígyós játék
Egy egyszerű és átlagos kígyós játék.
### [Forráskód](https://github.com/tlevi101/snake-java)

## C#/WPF Kígyós játék
Úgyanazokat a funkciókat implementálja mint a JAVA verzió, csak átfordítottam C#-ra.
### [Forráskód](https://github.com/tlevi101/snake-cs)

## PC monitoring webserver (C#)
Ez egy pici webserver ami a gépemnek a statisztikáit monitorozza, és azt egy szerveren elérhetővég teszi. Eredetileg WalpaperEngine-hez készült, annak segítségev HTML kódot be lehet állítani háttérképként, és így ott megtudom jeleníteni az adatokat. Sajnos félbe maradt, mert az egyedi mod amit csináltam a gépemhez és amihez kellett azt szét kellett szendem, ezútán nem kellett többé ezt használnom.
### [Forráskód](https://github.com/tlevi101/PCMonitoringConsoleApp)
