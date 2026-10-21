# MinArbetstid – webbapp för iPhone

## Funktioner
- Projekt och summering av timmar/mil per projekt och totalt
- Arbetstid antingen som direkt antal timmar eller start/slut med rast
- Körda mil direkt eller beräknat från mätarställning före/efter (km / 10)
- Historik, filtrering, CSV-export och JSON-säkerhetskopia/återställning
- PWA-filer för hemskärmsinstallation och enkel offline-cache

## Viktigt om lagring
Data sparas i localStorage i webbläsaren på den här enheten. Det är beständig lokal lagring, men inte en serverbackup och synkas inte mellan enheter. Safari-data kan rensas av användaren/iOS. Använd regelbundet Säkerhetskopia. För arbetskritisk användning rekommenderas en backend/databas och autentisering.

## Publicering krävs för hemskärmsinstallation
En PWA behöver normalt ligga på en HTTPS-adress. Lägg upp filerna i denna mapp på en statisk webbhost (t.ex. GitHub Pages, Netlify eller liknande). Efter publicering:
1. Öppna HTTPS-adressen i Safari på iPhone.
2. Tryck på Dela.
3. Välj Lägg till på hemskärmen.
4. Bekräfta namnet MinArbetstid och tryck Lägg till.

Öppna sedan appikonen från hemskärmen. Registreringar sparas separat i den installerade webbappens lokala webbläsarlagring. Exportera en JSON-säkerhetskopia regelbundet.

## Filer
- index.html – appen
- manifest.json – PWA-metadata
- sw.js – enkel offline-cache
- icon.svg – appikon
