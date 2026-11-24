# EasyConnect

<p align="center">
  <img src="https://img.shields.io/badge/version-5.3-blue" alt="Version">
  <img src="https://img.shields.io/badge/.NET-8.0-purple" alt=".NET">
  <img src="https://img.shields.io/badge/platform-Windows-lightgrey" alt="Platform">
  <img src="https://img.shields.io/badge/license-MIT-green" alt="License">
</p>

**A lightweight desktop app for IT professionals and power users.**  
Manage SSH hosts, RDP connections and websites in one clean window. All data stays on your PC.

---

## English

### Features

- **SSH & RDP** – Quick connect with custom ports (double-click or Enter)
- **Website monitoring** – Automatic status checks (green = online, red = offline)
- **Search** – Instant filter by name, host, note or group
- **Notes & Groups** – Organize hosts with tags (Prod, Home, Lab…)
- **Last used** – Recently connected hosts rise to the top
- **Ping** – Continuous ping for any selected host (right-click → Ping)
- **SSH Tunnels** – Create local port forwards with history
- **Backup** – Export / Import everything as `.ecbackup`
- **Shortcuts** – `F5` refresh · `Ctrl+F` search · `Del` remove · `Enter` connect

### SSH Tunnel (quick guide)

1. Right-click an SSH host → **Create Tunnel**
2. Fill in:
   - **Local Port** (e.g. `5400`)
   - **Remote Host** (e.g. `192.168.32.143`)
   - **Remote Port** (e.g. `80` or `5380`)
3. The app runs:  
   `ssh -L 5400:192.168.32.143:5380 -N user@ssh-host`
4. Open `http://localhost:5400` in your browser
5. Previous tunnels are saved in history

### Installation

**From installer (recommended)**  
Download `EasyConnect_Setup.exe` from [Releases](../../releases) and run it.

**Portable**  
Download the single-file `Easy_Connect.exe` and run it. No installation needed.

### Build from source

```bash
git clone https://github.com/YOUR_USERNAME/EasyConnect.git
cd EasyConnect
dotnet publish -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true
```

### Data location

All hosts and settings are stored in:  
`%AppData%\EasyConnect\`

---

## Suomi

**Kevyt työpöytäsovellus IT-ammattilaisille.**  
Hallitse SSH-palvelimia, RDP-yhteyksiä ja verkkosivustoja yhdessä ikkunassa. Kaikki tiedot pysyvät omalla koneellasi.

### Ominaisuudet

- Nopea SSH- ja RDP-yhteys (kaksoisklikkaus tai Enter)
- Verkkosivustojen automaattinen tilaseuranta
- Haku, muistiinpanot ja ryhmät
- Jatkuva ping valitulle palvelimelle
- SSH-tunnelit historialla
- Varmuuskopiointi `.ecbackup`-tiedostona
- Pikanäppäimet: `F5`, `Ctrl+F`, `Del`, `Enter`

### SSH-tunneli

1. Klikkaa SSH-palvelinta hiiren oikealla → **Create Tunnel**
2. Syötä paikallinen portti, etäpalvelin ja etäportti
3. Avaa selaimessa `http://localhost:PORT`

---

## Svenska

**Ett lättviktigt skrivbordsprogram för IT-proffs.**  
Hantera SSH-värdar, RDP-anslutningar och webbplatser i ett fönster. All data stannar på din dator.

### Funktioner

- Snabb SSH- och RDP-anslutning (dubbelklick eller Enter)
- Automatisk statuskontroll av webbplatser
- Sök, anteckningar och grupper
- Kontinuerlig ping för vald värd
- SSH-tunnlar med historik
- Export/import som `.ecbackup`
- Kortkommandon: `F5`, `Ctrl+F`, `Del`, `Enter`

### SSH-tunnel

1. Högerklicka på en SSH-värd → **Create Tunnel**
2. Ange lokal port, fjärrvärd och fjärrport
3. Öppna `http://localhost:PORT` i webbläsaren

---

## Русский

**Лёгкое настольное приложение для IT-специалистов.**  
Управление SSH-хостами, RDP-подключениями и сайтами в одном окне. Все данные остаются на вашем компьютере.

### Возможности

- Быстрое подключение по SSH и RDP (двойной клик или Enter)
- Автоматическая проверка статуса сайтов
- Поиск, заметки и группы
- Непрерывный пинг выбранного хоста
- SSH-туннели с историей
- Экспорт/импорт в формате `.ecbackup`
- Горячие клавиши: `F5`, `Ctrl+F`, `Del`, `Enter`

### SSH-туннель

1. Правый клик по SSH-хосту → **Create Tunnel**
2. Укажите локальный порт, удалённый хост и порт
3. Откройте в браузере `http://localhost:PORT`

---

## Deutsch

**Eine schlanke Desktop-Anwendung für IT-Profis.**  
Verwalte SSH-Hosts, RDP-Verbindungen und Websites in einem Fenster. Alle Daten bleiben auf deinem PC.

### Funktionen

- Schnelle SSH- und RDP-Verbindung (Doppelklick oder Enter)
- Automatische Statusprüfung von Websites
- Suche, Notizen und Gruppen
- Dauerhafter Ping für ausgewählten Host
- SSH-Tunnel mit Verlauf
- Export/Import als `.ecbackup`
- Tastenkürzel: `F5`, `Strg+F`, `Entf`, `Enter`

### SSH-Tunnel

1. Rechtsklick auf einen SSH-Host → **Create Tunnel**
2. Lokalen Port, Remote-Host und Remote-Port eingeben
3. Im Browser `http://localhost:PORT` öffnen

---

## License

MIT License — free for personal and commercial use.

Created by **Alexei Haikonen**
