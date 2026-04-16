# Duketown-NL UmbrelOS Store

Community app store voor UmbrelOS by Duketown-NL.

## Apps

### 🎮 Crafty Controller
Minecraft server manager — gefixed voor UmbrelOS.

De originele Crafty app geeft een `ECONNRESET` fout op UmbrelOS omdat de app proxy probeerde verbinding te maken via poort 8443 (HTTPS), terwijl Crafty's HTTP interface op poort 8000 draait. Deze versie gebruikt poort 8000 zodat de app direct werkt vanuit het Umbrel dashboard.

**Fix:** `APP_PORT` veranderd van `8443` naar `8000`

## Installatie

Voeg deze store toe in UmbrelOS:

1. Ga naar **App Store** in UmbrelOS
2. Klik op de **⋮** (drie puntjes) rechtsboven
3. Kies **Community App Stores**
4. Voeg toe:
```
https://github.com/DuketownNL/duketown-umbrel-store
```

## Eerste login Crafty

Na installatie vind je de standaard inloggegevens in:
```
data/config/default-creds.txt
```
Toegankelijk via het UmbrelOS bestandssysteem of via SSH.

## Credits

- Originele Crafty app: [Luna-OS](https://github.com/Luna-OS/mino-store-umbrelOS)
- Fix & store: [Duketown-NL](https://github.com/DuketownNL)
