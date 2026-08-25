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

## Home Assistant

Home Assistant is an open source smart home platform — I have nothing to do with
its development. However, my own setup has grown complex enough over the past
year that I think it's worth mentioning here.

**Infrastructure.** Home Assistant runs on my own Proxmox host. Next to it I run
a local voice assistant pipeline: a privileged LXC container with GPU passthrough
(NVIDIA device node bind-mounts) running `wyoming-faster-whisper` and
`wyoming-piper` in Docker. Speech-to-text and text-to-speech stay entirely on my
hardware instead of going to a cloud provider, and run on the GPU rather than
falling back to CPU.

**Protocols and devices.** The setup spans Zigbee, Thread/Matter, WiFi and
ESP-based devices — WLED light strips on ESP32, Nanoleaf Matter-over-Thread
bulbs, Zigbee sensors and buttons, a self-built mmWave presence sensor, and a
climate zone setup with derived comfort sensors.

**Automation architecture.** I migrated the system from scenes to explicit
scripts, which made lighting state — especially WLED presets driven through
`select.select_option` — deterministic and reusable instead of a pile of
snapshots.

**Debugging.** A large part of the work was diagnosis rather than configuration:
tracking a 2.4 GHz reliability problem down to SNR collapse from a charger in the
router's near field plus USB 3.0 emission, resolving Zigbee instability caused by
coordinator/USB adapter issues and co-channel interference with a Thread border
router, and chasing a WLED fault down to a failing ESP32.

**Beyond the smart home.** The same host runs Jellyfin as a personal streaming
service. A cron job watches the series directory, and when something new appears
it invokes the Claude Code CLI to decide what to do with it — whether the series
already exists, which season it belongs to — keeping the library consistently
organized with human-readable names. Ambient lighting driven by HyperHDR reacts
to what's on the TV screen.

What I take from this: most of the effort here was systems work, not smart home
work — Linux and container administration, RF and network troubleshooting,
building and soldering my own microcontroller devices, and designing an
automation layer that stays maintainable as it grows.

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

## Home Assistant

A Home Assistant egy nyílt forráskódú okosotthon platform — a fejlesztéséhez
semmi közöm. A saját rendszerem viszont az elmúlt egy évben elég összetetté vált
ahhoz, hogy szerintem érdemes itt megemlíteni.

**Infrastruktúra.** A Home Assistant a saját Proxmox hostomon fut. Mellette egy
helyi hangasszisztens pipeline is működik: egy privilegizált LXC konténer GPU
passthrough-val (NVIDIA device node bind-mountokkal), amiben a
`wyoming-faster-whisper` és a `wyoming-piper` fut Dockerben. Így a beszéd-szöveg
és szöveg-beszéd átalakítás teljes egészében a saját hardveremen marad, nem
felhőszolgáltatónál, ráadásul ténylegesen a GPU-n fut, nem esik vissza CPU-ra.

**Protokollok és eszközök.** A rendszer Zigbee, Thread/Matter, WiFi és ESP-alapú
eszközöket fog össze — ESP32-n futó WLED LED-szalagok, Nanoleaf
Matter-over-Thread izzók, Zigbee szenzorok és gombok, egy saját építésű mmWave
jelenlétérzékelő, valamint egy klímazóna-felállás származtatott
komfortszenzorokkal.

**Automatizálási architektúra.** A rendszert scene-ekről explicit scriptekre
migráltam, amitől a világítás állapota — különösen a `select.select_option`-nel
vezérelt WLED presetek — determinisztikussá és újrafelhasználhatóvá vált a
korábbi pillanatképek halmaza helyett.

**Hibakeresés.** A munka nagy része nem konfigurálás volt, hanem diagnosztika:
egy 2,4 GHz-es stabilitási problémát az SNR beszakadásáig vezettem vissza, amit a
router közvetlen közelében lévő töltő és az USB 3.0 zavarkibocsátása okozott;
megoldottam a Zigbee hálózat instabilitását, ami a koordinátor/USB adapter
hibáiból és a Thread border routerrel való azonos csatornás interferenciából
eredt; egy WLED hibát pedig egy meghibásodott ESP32-ig követtem le.

**Az okosotthonon túl.** Ugyanezen a hoston fut a Jellyfin mint személyes
streaming szolgáltatás. Egy cron feladat figyeli a sorozatok könyvtárát, és ha
új tartalom jelenik meg, meghívja a Claude Code CLI-t, ami eldönti, mi legyen
vele — létezik-e már a sorozat, melyik évadhoz tartozik —, így a könyvtár
következetesen rendezett marad, beszédes nevekkel. A HyperHDR által vezérelt
ambient világítás pedig a TV képernyőjének tartalmára reagál.

Amit ebből elviszek: a munka nagy része nem okosotthonozás volt, hanem
rendszerszintű munka — Linux- és konténer-adminisztráció, rádiós és hálózati
hibakeresés, saját mikrokontrolleres eszközök építése és forrasztása, valamint
egy olyan automatizálási réteg megtervezése, ami növekedés közben is
karbantartható marad.

## Java Kígyós játék
Egy egyszerű és átlagos kígyós játék.
### [Forráskód](https://github.com/tlevi101/snake-java)

## C#/WPF Kígyós játék
Úgyanazokat a funkciókat implementálja mint a JAVA verzió, csak átfordítottam C#-ra.
### [Forráskód](https://github.com/tlevi101/snake-cs)

## PC monitoring webserver (C#)
Ez egy pici webserver ami a gépemnek a statisztikáit monitorozza, és azt egy szerveren elérhetővég teszi. Eredetileg WalpaperEngine-hez készült, annak segítségev HTML kódot be lehet állítani háttérképként, és így ott megtudom jeleníteni az adatokat. Sajnos félbe maradt, mert az egyedi mod amit csináltam a gépemhez és amihez kellett azt szét kellett szendem, ezútán nem kellett többé ezt használnom.
### [Forráskód](https://github.com/tlevi101/PCMonitoringConsoleApp)
