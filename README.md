# Home Route – Downloads

Fahre und laufe durch echte Orte, gebaut auf deinem PC aus offenen Kartendaten.
*Drive and walk through real places, built on your PC from open map data.* → [English below](#english)

**[➜ Neueste Version herunterladen / Download the latest version](https://github.com/mimiundmomotv-wq/HomeRoute-Releases/releases/latest)**

---

## Deutsch: Installation Schritt für Schritt

### Was du brauchst
- Einen PC mit **Linux** (64 Bit). Windows und Mac gehen noch nicht.
- Eine Grafikkarte mit aktuellem Treiber (Vulkan). Bei AMD- und Intel-Grafik ist das unter Ubuntu, Fedora usw. meist schon dabei. Bei NVIDIA: den NVIDIA-Treiber installieren (Ubuntu: *Anwendungen & Aktualisierungen → Zusätzliche Treiber*).
- Mindestens 16 GB Arbeitsspeicher, etwa 1 GB freien Platz für das Spiel und einige GB pro selbst gebautem Gebiet.
- Für **neue Gebiete**: Internet und eine aktuelle Linux-Version, z. B. **Ubuntu 24.04** oder neuer, Debian 13, Fedora 39 oder neuer. Auf älteren Versionen (z. B. Ubuntu 22.04, Linux Mint 21) startet das Spiel und das Startdorf läuft, aber neue Gebiete lassen sich noch nicht bauen.

### 1. Herunterladen
1. Öffne die Seite **[Neueste Version](https://github.com/mimiundmomotv-wq/HomeRoute-Releases/releases/latest)**.
2. Scrolle nach unten zu **Assets**.
3. Klicke auf **`HomeRoute-…-Linux-x86_64.tar.gz`** (die große Datei, einige hundert MB).
   Die Einträge „Source code (zip)“ und „Source code (tar.gz)“ brauchst du **nicht**; GitHub hängt sie automatisch an, sie enthalten nur diese Anleitung.
4. Die Datei landet normalerweise im Ordner **Downloads**.

### 2. Entpacken
1. Öffne den Ordner **Downloads** im Dateimanager.
2. Rechtsklick auf die Datei `HomeRoute-…-Linux-x86_64.tar.gz` → **„Hier entpacken“** (oder „Entpacken“ / „Extract here“).
3. Es entsteht ein Ordner `HomeRoute-…-Linux-x86_64`. Du kannst ihn verschieben, wohin du willst (z. B. in deinen Home-Ordner). Die `.tar.gz`-Datei kannst du danach löschen.

### 3. Starten
1. Öffne den entpackten Ordner.
2. Doppelklick auf **`HomeRoute.sh`**.
   - **KDE (Dolphin):** Falls gefragt wird, **„Ausführen“** wählen.
   - **GNOME/Ubuntu (Dateien):** Öffnet sich stattdessen ein Texteditor, schließe ihn und mache einen Rechtsklick auf `HomeRoute.sh` → **„Als Programm ausführen“**.
   - **Klappt das nicht**, nimm das Terminal: Rechtsklick in den Ordner → „Im Terminal öffnen“, dann eintippen und Enter drücken:
     ```
     ./HomeRoute.sh
     ```
3. Der erste Start dauert etwas länger (bis zu einer Minute), weil die Grafik vorbereitet wird. Danach geht es schneller.

### 4. Spielen
- **Erstes Mal:** „Choose area“ → „Starter Town“ → **„Drive“**. Das ist ein ausgedachtes Dorf, sofort spielbar.
- **Deinen Ort bauen:** „New area“ → Ort oder Straße eintippen → „Search“ → Treffer anklicken → Größe wählen → **„Create area“**. Die Daten werden geladen und gebaut, das dauert je nach Größe einige Minuten. Am besten klappt es in **Nordrhein-Westfalen**, andere Bundesländer so weit es dort offene 3D-Gebäudedaten gibt.
- **Ruckelt es?** Im Menü „Settings“ die Stufe **Low** wählen.

**Tasten**

| Taste | Was sie tut |
|---|---|
| W / S | Gas / Bremse (zu Fuß: vor / zurück) |
| A / D | Lenken (zu Fuß: seitwärts) |
| Leertaste | Handbremse (zu Fuß: springen) |
| Maus | Umsehen |
| F | Aussteigen / Einsteigen |
| C | Auto zu dir rufen |
| R | Auto zurücksetzen |
| H | Zurück zum Start |
| Tab | Karte: Ort anklicken oder Straße suchen, um dorthin zu springen |
| V | Fliegen (F landet wieder zu Fuß) |
| M | Stelle markieren, mit Kommentar (für Fehlermeldungen) |
| Esc | Menü |

### Wo liegen meine Daten? Deinstallieren
- Selbst gebaute Gebiete und Einstellungen liegen in `~/.config/Epic/HomeRoute/` (versteckter Ordner im Home-Ordner; im Dateimanager mit **Strg+H** sichtbar machen).
- **Deinstallieren:** den Ordner `HomeRoute-…-Linux-x86_64` löschen. Wer auch Gebiete und Einstellungen loswerden will, löscht zusätzlich `~/.config/Epic/HomeRoute/`.
- **Neue Version:** einfach die neue Version herunterladen und entpacken; deine Gebiete bleiben erhalten.

### Wenn etwas nicht klappt
- **Startet nicht / schwarzes Bild:** Grafiktreiber aktualisieren (siehe „Was du brauchst“). Im Terminal starten (`./HomeRoute.sh`), dann siehst du eine Fehlermeldung.
- **„Create area“ bricht sofort ab:** Linux-Version zu alt (siehe oben) oder keine Internetverbindung.
- **Fehler melden:** Oben auf dieser Seite auf **Issues → New issue** klicken und beschreiben, was passiert ist (gern mit Bildschirmfoto). Bitte keine eigenen Adressen posten, wenn du das nicht möchtest.

*Prüfsumme (für Fortgeschrittene, optional):* Lade auch die `.sha256`-Datei in denselben Ordner und tippe dort `sha256sum -c HomeRoute-*.tar.gz.sha256` – es muss „OK“ erscheinen.

---

<a id="english"></a>
## English: step-by-step installation

### What you need
- A **Linux** PC (64-bit). Windows and Mac are not supported yet.
- A graphics card with a current driver (Vulkan). AMD and Intel graphics usually work out of the box on Ubuntu, Fedora etc. For NVIDIA, install the NVIDIA driver (Ubuntu: *Software & Updates → Additional Drivers*).
- At least 16 GB of RAM, about 1 GB of free disk space for the game, plus a few GB for each area you build.
- For **new areas**: an internet connection and a recent Linux, e.g. **Ubuntu 24.04** or newer, Debian 13, Fedora 39 or newer. On older ones (e.g. Ubuntu 22.04, Linux Mint 21) the game and the starter town work, but new areas can't be built yet.

### 1. Download
1. Open the **[latest version](https://github.com/mimiundmomotv-wq/HomeRoute-Releases/releases/latest)** page.
2. Scroll down to **Assets**.
3. Click **`HomeRoute-…-Linux-x86_64.tar.gz`** (the big file, a few hundred MB).
   You do **not** need "Source code (zip)" or "Source code (tar.gz)": GitHub adds them automatically and they only contain this guide.
4. The file usually ends up in your **Downloads** folder.

### 2. Unpack
1. Open **Downloads** in your file manager.
2. Right-click `HomeRoute-…-Linux-x86_64.tar.gz` → **"Extract here"**.
3. You get a folder `HomeRoute-…-Linux-x86_64`. Move it wherever you like; you can delete the `.tar.gz` afterwards.

### 3. Start
1. Open the unpacked folder.
2. Double-click **`HomeRoute.sh`**.
   - **KDE (Dolphin):** if asked, choose **"Execute"**.
   - **GNOME/Ubuntu (Files):** if a text editor opens instead, close it, right-click `HomeRoute.sh` → **"Run as a Program"**.
   - **If that doesn't work**, use a terminal: right-click inside the folder → "Open in Terminal", type this and press Enter:
     ```
     ./HomeRoute.sh
     ```
3. The first start takes a little longer (up to a minute) while the graphics are prepared.

### 4. Play
- **First time:** "Choose area" → "Starter Town" → **"Drive"**: a made-up village, playable at once.
- **Build your own place:** "New area" → type a town or street → "Search" → click a result → choose the size → **"Create area"**. The data is downloaded and built, which takes a few minutes depending on the size. Works best in **North Rhine-Westphalia** (Germany); other German states as far as they publish open 3D building data.
- **Choppy?** Choose **Low** in "Settings".

**Keys:** W/S drive and brake (on foot: forward/back), A/D steer, Space handbrake (on foot: jump), mouse look, F get out/in, C call the car, R reset the car, H back to start, Tab map (click a place or search a street to jump there), V fly (F lands on foot), M mark a spot with a comment, Esc menu.

### Your data, uninstalling, updating
- Your areas and settings are in `~/.config/Epic/HomeRoute/` (a hidden folder in your home folder; **Ctrl+H** shows hidden files).
- **Uninstall:** delete the `HomeRoute-…-Linux-x86_64` folder, and `~/.config/Epic/HomeRoute/` too if you want your areas and settings gone.
- **Update:** download and unpack the new version; your areas are kept.

### If something goes wrong
- **Doesn't start / black screen:** update your graphics driver; start it from a terminal (`./HomeRoute.sh`) to see the error.
- **"Create area" stops right away:** Linux too old (see above) or no internet.
- **Report a problem:** click **Issues → New issue** at the top of this page and describe what happened (a screenshot helps).

*Checksum (optional):* put the `.sha256` file next to the archive and run `sha256sum -c HomeRoute-*.tar.gz.sha256`; it should print "OK".

---
Licences: game code MIT, own assets CC BY-SA 4.0 / CC0. Map data © OpenStreetMap contributors (ODbL); geodata of the German states under their open licences (see Credits in the game). Built with Unreal Engine. This repository only holds the downloads.
