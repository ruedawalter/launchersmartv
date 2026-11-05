<p align="center">
  <a href="https://cleanyour.tv"><img src="https://raw.githubusercontent.com/Gathin23/cleanyourtv/main/docs/banner.png" alt="CleanYourTV. Your TV, minus the ads. Strip the bloatware from any Android TV or Google TV over Wi-Fi and replace the ad-filled home screen with a clean launcher that looks like an Apple TV. No root, no cable, nothing uninstalled, and a one-line restore." width="800"></a>
</p>

<p align="center">
  Leer en: <a href="README.zh-CN.md">简体中文</a> · <a href="README.zh-TW.md">正體中文</a> · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.ja.md">日本語</a> · <a href="README.it.md">Italiano</a> · <a href="README.nl.md">Nederlands</a>
</p>

<p align="center">
  <a href="https://github.com/Gathin23/cleanyourtv/stargazers"><img src="https://img.shields.io/github/stars/Gathin23/cleanyourtv?style=flat&cacheSeconds=1800&color=cfffcf&labelColor=15181e" alt="Stars"></a>
  <a href="https://github.com/Gathin23/cleanyourtv/pulls?q=is%3Amerged"><img src="https://img.shields.io/github/issues-search?query=repo%3AGathin23%2Fcleanyourtv%20is%3Apr%20is%3Amerged&style=flat&cacheSeconds=1800&label=merged%20PRs&color=cfffcf&labelColor=15181e" alt="Merged PRs"></a>
  <a href="https://github.com/Gathin23/cleanyourtv/network/members"><img src="https://img.shields.io/github/forks/Gathin23/cleanyourtv?style=flat&cacheSeconds=1800&color=cfffcf&labelColor=15181e" alt="Forks"></a>
  <a href="https://github.com/Gathin23/cleanyourtv/graphs/contributors"><img src="https://img.shields.io/github/contributors/Gathin23/cleanyourtv?style=flat&cacheSeconds=1800&color=cfffcf&labelColor=15181e" alt="Contributors"></a>
  <a href="https://buymeacoffee.com/gathint"><img src="https://img.shields.io/badge/support-%E2%9D%A4-ff5e8a?style=flat&labelColor=15181e" alt="Support, buy me a coffee"></a>
  <a href="https://www.producthunt.com/products/cleanyourtv"><img src="https://img.shields.io/badge/Product%20Hunt-upvote%20%E2%96%B2-da552f?style=flat&logo=producthunt&logoColor=white&labelColor=15181e" alt="CleanYourTV on Product Hunt"></a>
</p>

<p align="center">
  <a href="https://trendshift.io/repositories/310225"><img src="docs/trending-badge.png" alt="#1 trending repo of the week, Oct 19–25 2026, via trendshift.io" width="360"></a>
</p>

<p align="center">
  <a href="docs/PRESS.md"><img src="docs/card.jpg" alt="345 TV models · 93 brands · 29 languages · 532 KB launcher. Featured in TechCrunch, TechRadar, Tom's Guide, Mashable, Android Authority, XDA, FlatpanelsHD, It's FOSS, Phandroid, GIGAZINE, Xataka, WinFuture, Frandroid, Macitynet, Techaeris, TechPP and 297 more: 313 articles from 44 countries. Before: stock Google TV home with a sponsored ad. After: the Clean Your TV launcher." width="800"></a>
</p>

## Guía de instalación

Lee la [guía de instalación de CleanYourTV](docs/INSTALLATION_GUIDE.md) before installing the project.

## Comienza aquí

| Lo que tienes | Ve a |
|---|---|
| **Un Android TV o Google TV** | [Quick start](#quick-start): un asistente de programación hace el trabajo en unos quince minutos. |
| **Un televisor Samsung, LG, Roku, Vizio o Hisense VIDAA** | [cleanyour.tv/not-android](https://cleanyour.tv/not-android): CleanYourTV no puede ejecutarse allí, pero puedes desactivar el seguimiento con el control remoto. |
| **Solo un teléfono Android** | The community-built [Clean Your TV app](https://cleanyour.tv/app): sin computadora portátil ni asistente de programación. |
| **Quieres verlo antes** | [What you get](#what-you-get): capturas de pantalla de la nueva pantalla de inicio. |

**Enlaces oficiales:** [cleanyour.tv](https://cleanyour.tv) and this repo. Otros dominios que usan ese nombre, como
cleanyourtv.com, no pertenecen a este proyecto ([#1004](https://github.com/Gathin23/cleanyourtv/issues/1004)).

[How it works](#how-it-works) · [Quick start](#quick-start) · [What you get](#what-you-get) ·
[Supported TVs](#supported-tvs) · [Doing it by hand](#doing-it-by-hand) · [The launcher](#the-launcher) ·
[Restoring](#restoring-your-tv) · [Firmware updates](#after-a-firmware-update) ·
[Questions](#questions-people-ask) · [Contributing](#contributing)

## Cómo funciona

Los televisores Android tienen el mismo puente de depuración que los teléfonos Android. Activa la depuración USB en las
opciones de desarrollador del televisor, autoriza tu computadora una sola vez y el resto se realiza con herramientas estándar de Android:

| Paso | Qué sucede |
|---|---|
| **Crear una copia de seguridad** | Se guarda la lista de paquetes instalados y la configuración. |
| **Desactivar** | Se desactivan la telemetría del fabricante, los servicios de anuncios, las filas de contenido y las aplicaciones preinstaladas innecesarias mediante `pm disable-user`. No se desinstala nada, por lo que un script de restauración puede revertir cada paso. |
| **Instalar** | Se instala un launcher nativo ligero y se establece como pantalla de inicio predeterminada. |

**Sin root, sin cables, sin desinstalar nada y con una restauración de una sola línea si cambias de opinión.**

El software innecesario varía según la marca, por eso las instrucciones hacen que el asistente de programación lo identifique en tu televisor y pregunte
antes de modificar cualquier elemento que puedas utilizar.

## Inicio rápido

| Lo que tienes | Qué debes hacer |
|---|---|
| **Una computadora** | Usa las instrucciones con un asistente de programación y sigue los tres pasos siguientes. |
| **Una computadora, sin asistente de programación** | Realiza los tres pasos manualmente: los comandos están en [Hacerlo manualmente](#doing-it-by-hand). |
| **Solo un teléfono Android** | Use the community-built [Clean Your TV app](https://cleanyour.tv/app) by [@udhaykumarbala](https://github.com/udhaykumarbala): connect, analyse, clean, in about five minutes. No laptop, no coding agent. |

Los tres pasos siguientes están pensados para un asistente de programación: la computadora debe estar conectada a la misma red Wi-Fi que
el televisor y debes disponer de una terminal. Si no utilizas un asistente, [Doing it by hand](#doing-it-by-hand) puedes realizar el mismo procedimiento
por tu cuenta.

Any of these work: Claude Code (on [0G Private Computer](https://pc.0g.ai/?utm_source=cleanyourtv&utm_medium=github&utm_campaign=readme) or an [Anthropic plan](https://claude.com/pricing)), [Codex](https://github.com/openai/codex), [Gemini CLI](https://github.com/google-gemini/gemini-cli) or [Antigravity CLI](https://antigravity.google/product/antigravity-cli).

| Dónde | Qué hacer |
|---|---|
| **1. En el televisor** | Settings → Device Preferences → About → press OK on **Build** seven times → back → Developer options → **USB debugging** on. If you see a Network or ADB debugging toggle, turn that on too. Keep the TV on. |
| **2. En tu computadora** | Clone the repo and open that folder in your assistant (`git clone https://github.com/Gathin23/cleanyourtv`), then paste [`PROMPT.md`](PROMPT.md) and fill in your TV model. |
| **3. Sigue las instrucciones** | Acepta «¿Permitir la depuración USB?» en el televisor y responde la lista de preguntas: qué aplicaciones utilizas, el tamaño del dock y el orden de las aplicaciones, y si deseas conservar el asistente de voz, Chromecast y las actualizaciones. |

Clonar el repositorio es importante: el asistente reutiliza los archivos `tools/disable.sh` and `launcher/build-and-install.sh`
de este proyecto en lugar de crear sus propias versiones. Allí se encuentran la copia de seguridad, la protección de Home y el registro de restauración.

El asistente crea una copia de seguridad, elimina el software innecesario, compila e instala el launcher y comprueba cada paso mediante
capturas de pantalla obtenidas del televisor. Con este repositorio como referencia, el proceso tarda unos quince minutos.

## Qué obtienes

Una pantalla de inicio con apariencia de Apple TV, sencilla y sin elementos molestos:

| Elemento | Descripción |
|---|---|
| **Una pantalla de inicio completamente negra** | Un dock con tus cuatro aplicaciones favoritas dentro de una banda redondeada, como en Apple TV. |
| **Una sección superior** | Muestra en letras grandes el nombre de la aplicación seleccionada, con un resplandor ambiental del color de su imagen. |
| **El resto de tus aplicaciones en una cuadrícula** | Aparece al pulsar Abajo. |
| **Un resaltado de cristal flotante** | Se desplaza entre los mosaicos. El mosaico seleccionado se eleva y muestra su nombre. |
| **Tres botones translúcidos** | Inputs (HDMI ports under the names you gave them in the TV's settings, AV, Live TV), Wi-Fi or Ethernet with the network name, Settings. |
| **Un saludo, un reloj minimalista y la fecha** | Con la fuente [Outfit](https://fonts.google.com/specimen/Outfit), and a matching Clock screensaver. Set `show_stats` in config or a theme for one line under the clock: CPU, free memory and free storage. It stays off unless you turn it on, and it refreshes only while Home is on screen. |
| **Temas y tarjetas de módulos** | Themes change colours, wallpaper, dock and columns without a rebuild, and module cards let other apps plug a tile in, only with your say-so. |

Y un televisor que deja de molestarte: sin filas patrocinadas, sin avisos de «Discover» y sin analítica
que envíe información a terceros ni aplicaciones que nunca solicitaste.

| | |
|---|---|
| ![The top shelf names the focused app over an ambient glow in its colour](docs/focus-2-up-netflix.png) | ![The Inputs popup: HDMI ports with what is connected, AV and Live TV](docs/inputs-menu.jpg) |
| *Top shelf and ambient glow* | *Inputs: HDMI with connection state, AV, Live TV* |
| ![The grid with the glass highlight on a tile and its name beneath](docs/focus-1-fancode.png) | ![The Clock screensaver: a thin clock drifting over the glow](docs/clock-screensaver.png) |
| *The grid, one glass highlight, the tile's name* | *Clock screensaver, drifts so nothing burns in* |
| ![The aurora theme: a wallpaper and tinted pills, pushed without a rebuild](themes/aurora/screenshot.jpg) | ![Six columns and a six-app dock from a theme's config.json](themes/six-columns/screenshot.jpg) |
| *Aurora theme, pushed with `tools/theme.sh`* | *Six columns and a six-app dock, same launcher* |
| ![Moving a tile: held OK, chose Move, the tile is picked up and the others dim](docs/tile-move.jpg) | ![The App library: installed apps, one press adds an app back to Home](docs/app-library.jpg) |
| *With `tile_menu`, hold OK on a tile, Move: arrows carry it, Back puts it down* | *App library: one press puts a removed app back on Home* |

## Televisores compatibles

Cualquier televisor que utilice **Android TV** o **Google TV**.

| Plataforma | Funcionalidad |
|---|---|
| **Android TV y Google TV** | La limpieza de aplicaciones y el launcher. |
| **Fire TV** | Solo funciona la parte de limpieza, ya que Fire OS no permite establecer un launcher de terceros como pantalla de inicio. And on the 2015 Fire TV Box (Fire OS 5) even that half fails: every `pm` route is refused. |
| **Algunos modelos TCL del mercado chino** | No permiten instalar ningún launcher; sus listas lo indican en el encabezado. |
| **Samsung (Tizen), LG (webOS), Roku, Vizio, Hisense VIDAA** | Not supported (no ADB). Turn off the tracking instead: [cleanyour.tv/not-android](https://cleanyour.tv/not-android). See [SHOWCASE.md](SHOWCASE.md#other-platforms-fire-tv-and-lg-webos) for four webOS ports, and [docs/devices/samsung-tizen.md](docs/devices/samsung-tizen.md) for what a 2021 Samsung set answers over Wi-Fi (no ADB, so no `pm disable-user`) if you are weighing a Tizen port. |

Tested lists from contributors, one folder per model in [`examples/`](examples/). The brands with the
most lists, each linked to its models on the website:

<!-- tv-brands:start: generated by tools/gen_tables.py from examples/*/tv.json; edit those, not this -->

| | | | | | |
|---|---|---|---|---|---|
| [TCL](https://cleanyour.tv/tvs?q=TCL) · 76 | [Sony](https://cleanyour.tv/tvs?q=Sony) · 40 | [Xiaomi](https://cleanyour.tv/tvs?q=Xiaomi) · 32 | [Philips](https://cleanyour.tv/tvs?q=Philips) · 18 | [Skyworth](https://cleanyour.tv/tvs?q=Skyworth) · 14 | [Hisense](https://cleanyour.tv/tvs?q=Hisense) · 11 |
| [Amazon Fire TV](https://cleanyour.tv/tvs?q=Amazon%20Fire%20TV) · 7 | [Panasonic](https://cleanyour.tv/tvs?q=Panasonic) · 6 | [BenQ](https://cleanyour.tv/tvs?q=BenQ) · 5 | [SHARP](https://cleanyour.tv/tvs?q=SHARP) · 5 | [JVC](https://cleanyour.tv/tvs?q=JVC) · 4 | [OnePlus](https://cleanyour.tv/tvs?q=OnePlus) · 4 |
| [Thomson](https://cleanyour.tv/tvs?q=Thomson) · 4 | [Google](https://cleanyour.tv/tvs?q=Google) · 3 | [Grundig](https://cleanyour.tv/tvs?q=Grundig) · 3 | [Haier](https://cleanyour.tv/tvs?q=Haier) · 3 | [Motorola](https://cleanyour.tv/tvs?q=Motorola) · 3 | [NVIDIA Shield](https://cleanyour.tv/tvs?q=NVIDIA%20Shield) · 3 |
| [RCA](https://cleanyour.tv/tvs?q=RCA) · 3 | [Redmi](https://cleanyour.tv/tvs?q=Redmi) · 3 | [Toshiba](https://cleanyour.tv/tvs?q=Toshiba) · 3 | [Vu](https://cleanyour.tv/tvs?q=Vu) · 3 | [CHiQ](https://cleanyour.tv/tvs?q=CHiQ) · 2 | [EKO](https://cleanyour.tv/tvs?q=EKO) · 2 |
| [FFalcon](https://cleanyour.tv/tvs?q=FFalcon) · 2 | [Hitachi](https://cleanyour.tv/tvs?q=Hitachi) · 2 | [Insignia Fire TV](https://cleanyour.tv/tvs?q=Insignia%20Fire%20TV) · 2 | [Kalley](https://cleanyour.tv/tvs?q=Kalley) · 2 | [Kogan](https://cleanyour.tv/tvs?q=Kogan) · 2 | [Nokia](https://cleanyour.tv/tvs?q=Nokia) · 2 |

<details>
<summary>+49 more brands and 14 projector brands</summary>

**onn** 2 · **RockTek** 2 · **Sankey** 2 · **Sber** 2 · **Vidda** 2 ·
Acer · AiPro2K · AIWA · AQUA · Artel · ASUS · Beko · BGH · Caxium · Cecotec · Challenger · Compac · Dcolor · Dialog ·
DYON · Freebox · Home+ · INCLO · Karbonn · KTC · Liberton · Lumio · Master-G · MTC · Next · Noblex · OK. · OPPO ·
Panavox · PEAQ · Polytron · PPTV · PRISM+ · SANYO · Seleco · Super General · Síragon · Tele System · TiVo · Tornado ·
Turkcell · Tuvio · Verizon · Vision ·
Alwtniet, Anker Nebula, BYINTEK, Epson, Formovie, Gadnic, HOTACK, HY320, JMGO, Magcubic, Portronics, Stellamore, Wanbo and XGIMI projectors

</details>

<!-- tv-brands:end -->

**Encuentra tu televisor:** busca [cleanyour.tv/tvs](https://cleanyour.tv/tvs) or the full table in
[examples/README.md](examples/README.md).

¿Tu televisor no aparece? Las instrucciones permiten detectar automáticamente las aplicaciones innecesarias. Después puedes añadir tu lista para que la siguiente
persona con ese modelo no tenga que repetir el proceso: [CONTRIBUTING.md](CONTRIBUTING.md).

## Hacerlo manualmente

Puedes realizar manualmente todo lo que hace el asistente. Las herramientas solo necesitan Python 3.
`tools/tv.py` talks to network ADB on port 5555. Si ese puerto permanece cerrado y el televisor ofrece
Wireless debugging with a pairing code (the Chromecast with Google TV and the Google TV Streamer
do), realiza el emparejamiento una vez con `adb` estándar y ejecuta primero `adb tcpip 5555`, tal como se explica en
[Troubleshooting](docs/TROUBLESHOOTING.md#connecting) describes.

```bash
python3 -m venv tools/venv && tools/venv/bin/pip install -r tools/requirements.txt
export TV_HOST=192.168.1.50                                   # your TV's IP address

tools/venv/bin/python -I tools/tv.py --probe                 # model, Android version, firmware
tools/venv/bin/python -I tools/tv.py 'pm list packages'      # one shell command on the TV
tools/disable.sh examples/xiaomi-mi-tv-4a/debloat.txt        # apply a debloat list
tools/restore.sh examples/xiaomi-mi-tv-4a/debloat.txt        # undo it, stock launcher back
tools/venv/bin/python -I tools/check.py examples/xiaomi-mi-tv-4a/debloat.txt   # what a firmware update undid
TV_HOST=192.168.1.50 launcher/build-and-install.sh           # build the launcher and make it Home
tools/theme.sh themes/aurora                                 # push a theme; --reset removes it
```

| Herramienta | Función |
|---|---|
| [`tools/tv.py`](tools/tv.py) | Pure-Python ADB client: shell, batch, push, pull, reboot, and screenshots, optionally pressing remote keys first. Works where the stock `adb` binary is blocked. Optional [paired Google ADB backend](tools/native-adb.md) for encrypted Wireless debugging. |
| [`tools/b64push.py`](tools/b64push.py) | Uploads large files such as APKs in base64 chunks and verifies the checksum. |
| [`tools/relay.py`](tools/relay.py) | Forwards a local port to the TV's ADB port, for assistants whose sandbox can't reach your network. Listens on this computer only. [Guide](tools/relay.md). |
| [`tools/disable.sh`](tools/disable.sh), [`restore.sh`](tools/restore.sh) | Apply or undo a debloat list, the undo from the state recorded before the change. |
| [`tools/recovery.py`](tools/recovery.py) | Writes the record `disable.sh` needs to undo itself, and prints the restore batch. |
| [`tools/check.py`](tools/check.py) | Compares the TV with the list that was applied, for what a firmware update undid; `--fix` puts it back. |
| [`tools/adb-closed.py`](tools/adb-closed.py) | Checks that the TV's network ADB port is closed once debugging is off: exits 0 when the TV refuses the connection, 1 while it is still open, 2 when nothing answered or the check itself could not run. No `nc` needed. |
| [`tools/privacy.py`](tools/privacy.py) | Audits the TV for voice, ACR and telemetry candidates and prints the evidence for each; `--write` turns the findings into a list `disable.sh` and `restore.sh` already understand. |
| [`tools/theme.sh`](tools/theme.sh), [`theme_restart.py`](tools/theme_restart.py) | Push a folder from [`themes/`](themes/) to the launcher and restart Home. |
| [`tools/manage.py`](tools/manage.py) | List every add-on, theme and switch with its screenshot, see what is on the TV, and install, update or remove one by running its creator's own script. |
| [`tools/bench.py`](tools/bench.py) | Measures the launcher that answers HOME: key latency, how far the focus moved, janky frames, cold start, return to Home, and the idle CPU and PSS it costs. Changes nothing on the TV and writes the raw per-key numbers to JSON; no extra install. |
| [`tools/trace.py`](tools/trace.py), [`trace_report.py`](tools/trace_report.py) | Records Perfetto traces of the launcher (return to Home, cold start, D-pad) and reports where its time goes, per run and before against after. Optional: needs [`requirements-perf.txt`](tools/requirements-perf.txt). [Guide](tools/trace.md). |
| [`tools/flamechart.py`](tools/flamechart.py) | Draws a before/after flame chart from those traces, for a pull request: one lane per thread on a shared time scale, the work a change targets in magenta with its total. Optional, like the trace tools. [Guide](tools/flamechart.md). |
| [`tools/screendiff.py`](tools/screendiff.py) | Compares a before and an after screenshot pixel by pixel, leaving out the clock or anything you mask, and writes the pair with your Wi-Fi name blurred. Optional, like the trace tools. [Guide](tools/screendiff.md). |
| [`tools/race_calendar.py`](tools/race_calendar.py) | Writes this season's F1 calendar into a theme for race-weekend mode, from the free Jolpica API. |
| [`launcher/build-and-install.sh`](launcher/build-and-install.sh) | Builds a shrunk release (about 532 KB), installs it, switches Home, and rolls back if Home does not land on it. |

Los scripts nunca dejan el televisor sin una aplicación Home: solo desactivan un launcher original reconocido
y omiten de la lista la aplicación Home hasta que otro launcher responda a HOME. Puedes guardar tus propias listas fuera
del repositorio: las rutas son relativas al directorio desde el que ejecutas el comando, aunque también se admiten rutas absolutas.

<details>
<summary><b>Windows (PowerShell)</b></summary>

Cada script tiene una versión equivalente para PowerShell. En Windows, con Android Studio instalado, no
necesitas nada más:

```powershell
python -m venv tools\venv; tools\venv\Scripts\python.exe -m pip install -r tools\requirements.txt
powershell -ExecutionPolicy Bypass -File launcher\build-and-install.ps1 -TvHost 192.168.1.50
powershell -ExecutionPolicy Bypass -File tools\disable.ps1 -TvHost 192.168.1.50 examples\xiaomi-mi-tv-4a\debloat.txt
```

</details>

<details>
<summary><b>How the scripts protect Home</b></summary>

The install scripts ask the TV which launcher owns Home and only disable one they recognise, the four
in `KNOWN_STOCK_LAUNCHERS`: `com.google.android.tvlauncher`, `com.google.android.apps.tv.launcherx`,
`com.google.android.leanbacklauncher` and Xiaomi's `com.mitv.tvhome` (PatchWall). Pass
`STOCK_LAUNCHER=<package>` (`-StockLauncher`) to override, or `none` to leave it alone.

`tools/disable.sh` (`disable.ps1`) applies the same rule before it disables anything:

- If the list contains the app that owns Home and no other app on the TV answers HOME, it skips that
  entry, says why, and disables the rest of the list. So a list applied before the launcher handover
  cannot leave the TV with nothing to start.
- The setup wizard, the settings apps, a vendor `FallbackHome` and factory-test apps (Xiaomi's
  `com.duokan.factorytest`) answer HOME too and don't count.
- On Google TV it also keeps the owner while setupwraith answers HOME and stays enabled (not listed, or
  kept for the Wi-Fi network): setupwraith answers ahead of an installed launcher that is not Home yet,
  so it would take Home.

Run the same list again once `launcher/build-and-install.sh` has made the new launcher Home and the
entry is applied; `FORCE_HOME=1` (`$env:FORCE_HOME`) disables it anyway.

</details>

## El micrófono y lo que podemos saber sobre él

"Which of these packages is listening?" no tiene una respuesta sencilla: un análisis de permisos puede mostrar cincuenta
paquetes del sistema con `RECORD_AUDIO` que no graban nada, mientras que los clientes ACR pueden analizar la pantalla sin necesitar permisos de audio
. [`tools/privacy.py`](tools/privacy.py) informa de lo que realmente indica el televisor y muestra las
pruebas de cada posible componente de voz, ACR y telemetría:
`TV_HOST=192.168.1.50 tools/venv/bin/python -I tools/privacy.py`, and `--write` turns them into a normal
debloat list. La auditoría no puede demostrar la intención de cada componente: [docs/privacy.md](docs/privacy.md) explains why.

## El launcher

Una pantalla de inicio nativa y ligera para Android TV: **aproximadamente 532 KB**, desarrollada en Java y diseñada para televisores con 1 GB de RAM.
No blur, no video, no network permission, no background services. The **TV** needs Android 8.0 (API 26)
or newer, the `minSdk` in [`launcher/app/build.gradle`](launcher/app/build.gradle); what is left on an older
set is in [Troubleshooting](docs/TROUBLESHOOTING.md).

| Característica | Funcionamiento |
|---|---|
| **Configuración** | Dock order, hidden apps, Live TV app, 4 to 7 tiles per row, reduced motion. All in [`config.xml`](launcher/app/src/main/res/values/config.xml) |
| **Ajustes en el televisor** | Hold OK on Settings for launcher settings. Optional `launcher_settings_button` makes a normal click open them directly; TV settings remain on the settings page and their app tile. |
| **Temas** | Background, wallpaper and layout from a `config.json` pushed over Wi-Fi, no rebuild. ten ship in [`themes/`](themes/), the built-in `default/` included |
| **29 idiomas** | Utiliza el idioma del televisor e incluye una interfaz adaptada de derecha a izquierda para hebreo |
| **Biblioteca de aplicaciones** | Optional: browse every installed app and add or remove Home shortcuts. See [the app library guide](docs/app-library.md) |
| **Menú de mosaicos** | Optional (`tile_menu`): hold OK on a tile for Move, Remove from Home and App info. Off, holding OK opens App info |
| **Tarjetas de módulos** | Any TV app can offer its own tile; you approve each one once. See [`docs/modules.md`](docs/modules.md) |
| **Complementos** | Optional apps that plug in as module cards, kept in [`addons/`](addons/) and never built into the launcher |
| **Salvapantallas de reloj** | A drifting clock over the glow, so nothing burns in |
| **Botones del control remoto** | Keeps the Input, YouTube and gear buttons working after the stock launcher is gone |

Temas, opciones y complementos, con capturas de pantalla: [cleanyour.tv/addons](https://cleanyour.tv/addons).

**Más información:** [docs/launcher.md](docs/launcher.md) has the launcher settings page row by row, changing the
default home, the languages, remote keys, the Clock screensaver, navigation and building it yourself.

## Restaurar el televisor

Conserva la lista que aplicaste. Un solo comando permite devolver el televisor a su estado anterior:

```bash
TV_HOST=192.168.1.50 tools/restore.sh examples/<your tv>/debloat.txt                                    # Android TV
TV_HOST=192.168.1.50 tools/restore.sh examples/<your tv>/debloat.txt com.google.android.apps.tv.launcherx  # Google TV
```

| Qué | Cómo |
|---|---|
| **Primero se crea un registro** | Antes de que `tools/disable.sh` modifique algo, guarda el estado original del televisor en `~/.cleanyourtv/`. |
| **La restauración recupera ese estado** | Los paquetes que ya habías desactivado manualmente permanecen desactivados y Home vuelve al componente que lo controlaba originalmente. |
| **El launcher permanece instalado** | Si deseas eliminarlo, hazlo desde Ajustes → Aplicaciones del televisor. |
| **¿No tienes una computadora?** | Si no puedes acceder al televisor, también puedes volver a habilitar los paquetes desde Ajustes → Aplicaciones. |

**Más información:** [docs/restore.md](docs/restore.md) has what the record holds, when the stock launcher argument
counts, and what happens without a record.

## Después de una actualización de firmware

Una actualización se instala sobre el sistema ya limpiado: los paquetes incluidos en la lista vuelven a aparecer y Home regresa al
launcher original. También pueden aparecer nuevas aplicaciones preinstaladas que no figuran en ninguna lista. Activa ADB nuevamente como se indica en
[Quick start](#quick-start) step 1, y compara el televisor con la lista aplicada; `--fix` restaura los cambios:

```bash
TV_HOST=192.168.1.50 tools/venv/bin/python -I tools/check.py examples/<your tv>/debloat.txt
```

**Más información:** [docs/firmware-updates.md](docs/firmware-updates.md) has the exit codes, a weekly check, what
`--fix` changes, TVs that keep the stock launcher as Home, and lists that disable the updater.

## Cuando algo sale mal

La lista completa de problemas conocidos está en [docs/TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md). The
three that matter most:

- 🍎 **macOS blocks `adb connect`** ("No route to host") under Local Network privacy. `tools/tv.py` avoids the binary.
- ⚠️ **Disable the stock launcher only after the new one is installed and running**, or Home lands on a factory test app. The install script orders this for you.
- 🔁 **On Google TV the setup wizard** (`com.google.android.tungsten.setupwraith`) can take Home and crash-loop the system after the stock launcher is disabled. Disable it too, and list it in your `debloat.txt` so restore brings it back.
  - But check `dumpsys wifi | grep -o 'cname=[^ ]*'` first: if the Wi-Fi network was saved during setup it belongs to setupwraith, and disabling it deletes the network (re-join it in Settings first; `tools/disable.sh` skips setupwraith until you do).
  - On Google's own Chromecast and on the Google TV Streamer it also costs phone casting, see [Troubleshooting](docs/TROUBLESHOOTING.md).
  - Stuck already? `tools/tv.py 'pm enable --user 0 com.google.android.apps.tv.launcherx'`.

## Preguntas frecuentes

<details>
<summary><b>No sé programar y no tengo una computadora portátil. ¿Puedo hacerlo?</b></summary>

Sí. [@udhaykumarbala](https://github.com/udhaykumarbala) desarrolló una [aplicación gratuita y de código abierto para teléfonos](https://cleanyour.tv/app)
para Android que realiza la misma limpieza mediante Wi-Fi: se conecta al televisor, muestra primero un plan, guarda un punto de restauración
y únicamente desactiva aplicaciones, por lo que todo se puede recuperar. Es un desarrollo de la comunidad.

</details>

<details>
<summary><b>¿Es seguro? ¿Puede dejar inutilizable el televisor?</b></summary>

No se instala firmware, no se obtiene acceso root ni se elimina nada; los paquetes se desactivan
en el perfil de usuario. El riesgo consiste en desactivar algún componente necesario para el televisor; por eso las listas se
aplican en grupos pequeños y siempre se dispone de un script de restauración. La propia sección Ajustes → Aplicaciones del televisor puede
volver a habilitar los paquetes incluso sin estas herramientas. Si el televisor no inicia lo suficiente para hacerlo, normalmente puedes realizar un
restablecimiento de fábrica desde el menú de recuperación.

More: [docs/faq.md](docs/faq.md#is-this-safe-can-it-brick-the-tv)

</details>

<details>
<summary><b>¿Qué ocurre con las actualizaciones de firmware?</b></summary>

En la mayoría de las listas, el actualizador permanece habilitado y las actualizaciones de firmware llegan normalmente. Algunas listas desactivan el
actualizador del propio televisor; en esos casos, solo recibirás actualizaciones cuando vuelvas a habilitarlo. Cuando se instala una actualización,
esta se aplica sobre el sistema limpiado, por lo que algunos paquetes reaparecen y debes ejecutar nuevamente el script. Consulta
[After a firmware update](#after-a-firmware-update).

</details>

<details>
<summary><b>¿Dejarán de funcionar las aplicaciones?</b></summary>

Las aplicaciones de streaming siguen actualizándose mediante Play Store, que no se modifica.
El launcher simplemente muestra las aplicaciones instaladas y las abre mediante mecanismos de Android que llevan una década siendo estables.

</details>

<details>
<summary><b>¿Puedo hacerlo para alguien que vive en otra casa?</b></summary>

Sí, mediante una conexión privada [Tailscale](https://tailscale.com)
en lugar de utilizar la misma red Wi-Fi: puedes instalar Tailscale en su televisor y compartir el acceso contigo, o utilizar una computadora o Apple
TV en su casa para enrutar la conexión. Nunca abras el puerto ADB en su router. Consulta la guía paso a paso en
[docs/REMOTE.md](docs/REMOTE.md).

</details>

<details>
<summary><b>¿El acceso ADB representa un riesgo de seguridad?</b></summary>

Solo requiere pulsar una vez «Permitir esta computadora» en el televisor, igual que al
desarrollar una aplicación Android. ADB por red transmite texto sin cifrar mediante el puerto 5555 y, en algunos firmwares, cualquier
dispositivo de la red local puede obtener acceso a una terminal. Por eso debes cerrarlo cuando termines:

1. On the TV: Developer options → turn **USB debugging**, **Network/ADB debugging** and
   **Wireless debugging** off, whichever the TV has, and revoke the USB debugging authorisations.
2. Reboot the TV, then confirm the port is gone from your computer:
   `python3 tools/adb-closed.py <tv ip>` must say the port is closed.

El launcher sigue funcionando aunque desactives la depuración. Más información, incluida la comprobación del puerto de Wireless debugging:
[docs/faq.md](docs/faq.md#isnt-adb-access-a-security-hole)

</details>

<details>
<summary><b>¿También puede bloquear anuncios dentro de las aplicaciones?</b></summary>

Parcialmente, mediante Private DNS de Android (Android 9 o superior). Configúralo para utilizar
un servicio DNS que bloquee anuncios, como [AdGuard DNS](https://adguard-dns.io) y los dominios de anuncios y
rastreadores de todas las aplicaciones dejarán de resolverse en todo el sistema, incluso después de reiniciar. La desventaja es que ese servicio DNS podrá ver
todas las consultas DNS del televisor y no elimina los anuncios de YouTube.

More, with the two commands and how to switch back: [docs/faq.md](docs/faq.md#can-it-block-ads-inside-apps-too)

</details>

<details>
<summary><b>¿Hay otras opciones en los ajustes del televisor que convenga desactivar?</b></summary>

Sí. Algunas no requieren ADB: el identificador de publicidad, la ubicación, el uso y diagnóstico y la búsqueda siempre
disponible, además del modo «Solo aplicaciones» cuando se conserva el launcher original. Desactiva Uso y diagnóstico antes de
realizar la limpieza; en algunos televisores esa sección también se desactiva.

More, with the paths for Google TV, Android TV and Fire OS:
[docs/faq.md](docs/faq.md#are-there-switches-in-the-tvs-own-settings-worth-flipping-too)

</details>

<details>
<summary><b>¿AirPlay?</b></summary>

Este repositorio no lo incluye. Chromecast integrado sigue disponible para teléfonos Android. Para iPhone,
[jqssun/android-airplay-server](https://github.com/jqssun/android-airplay-server) funciona; existe un script de instalación
en [PR #84](https://github.com/Gathin23/cleanyourtv/pull/84).

</details>

<details>
<summary><b>¿Puedo simplemente descargar el APK?</b></summary>

Compílalo con el script de una sola línea; tarda aproximadamente un minuto y así
tienes el control de lo que instalas en tu televisor. No se proporcionan binarios precompilados.

</details>

## La historia

El 17 de octubre de 2026 publiqué [un antes y un después](https://x.com/gathint/status/2111379569030939102) de la televisión de mis
padres, limpiada mediante Claude Code por Wi-Fi. La publicación alcanzó 7,4 millones de visualizaciones y otras personas comenzaron a hacer lo mismo con
sus televisores. Sus respuestas dieron origen a las listas de este repositorio: más de 170 modelos de televisores aportados por más de 200 colaboradores en cuatro
días. El repositorio se llamó tv-vibehack hasta el día 19; los enlaces antiguos siguen funcionando. La cobertura de prensa está disponible en
[docs/PRESS.md](docs/PRESS.md).

## Cómo contribuir

La contribución más útil es compartir la lista de limpieza de tu televisor, para que la siguiente persona con ese modelo no
tenga que volver a identificar las aplicaciones innecesarias. [CONTRIBUTING.md](CONTRIBUTING.md) explica el formato y las pruebas que solicitamos.
¿Vas a contribuir mediante un asistente de programación? [AGENTS.md](AGENTS.md) contiene las mismas reglas para el asistente.

| Cómo ayudar | En qué consiste |
|---|---|
| **La lista de limpieza de tu televisor** | Es la contribución más útil: la siguiente persona con ese modelo no tendrá que repetir la identificación. |
| **El launcher y las instrucciones** | También son bienvenidas las mejoras del launcher y de las instrucciones. |
| **¿Has creado algo basado en este proyecto?** | Un launcher, una adaptación o un tema: añádelo a [SHOWCASE.md](SHOWCASE.md), donde ya se recopilan 144 proyectos, organizados en pantallas de inicio, bifurcaciones, complementos, herramientas y otras plataformas, con un índice por marca de televisor. |

Personas que han contribuido a este repositorio:

<a href="https://github.com/Gathin23/cleanyourtv/graphs/contributors"><img src="https://contrib.rocks/image?repo=Gathin23/cleanyourtv&columns=16&max=400" alt="Contributors"></a>

<details>
<summary><strong>Star history</strong></summary>

<a href="https://star-history.com/#Gathin23/cleanyourtv&Date"><img src="https://api.star-history.com/svg?repos=Gathin23/cleanyourtv&type=Date" alt="Star history chart" width="640"></a>

</details>

## Contacto

| Motivo | Contacto |
|---|---|
| **Consultas sobre tu televisor** | [GitHub Discussions](https://github.com/Gathin23/cleanyourtv/discussions) |
| **Prensa y consultas** | [hello@itsgathin.com](mailto:hello@itsgathin.com) |
| **Problemas de seguridad** | Repórtalos de forma privada mediante la [Security tab](https://github.com/Gathin23/cleanyourtv/security), see [`SECURITY.md`](SECURITY.md) |

## Aviso legal

- CleanYourTV es un proyecto independiente de código abierto. No está afiliado, respaldado ni patrocinado
  por ningún fabricante de televisores ni plataforma. Los nombres de marcas y modelos se utilizan únicamente para indicar en qué televisores se probó cada lista,
  y siguen siendo marcas registradas de sus respectivos propietarios.
- Funciona únicamente mediante opciones que el propio televisor ofrece a su propietario: Opciones de desarrollador, depuración ADB y
  el comando `pm disable-user` de Android, equivalente a Ajustes > Aplicaciones > Desactivar. No obtiene acceso root al televisor,
  no instala firmware ni elude bloqueos, DRM o protecciones anticopia. El repositorio tampoco contiene
  software, firmware ni APK de fabricantes.
- No se desinstala nada y `tools/restore.sh` permite restaurar todos los cambios. Debes ejecutarlo en un televisor de tu propiedad y bajo tu
  propia responsabilidad. Modificar el software del televisor puede afectar su garantía o soporte técnico.
- Todo el contenido se proporciona «tal cual», sin ningún tipo de garantía, bajo la licencia MIT indicada a continuación.

## Licencia

MIT; consulta [`LICENSE`](LICENSE). La tipografía Outfit se distribuye bajo la SIL Open Font License; consulta
`launcher/FONT-LICENSE-OFL.txt`.
