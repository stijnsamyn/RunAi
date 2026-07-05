# RunAi webapp — online zetten in 10 minuten

De webapp is één bestand (`index.html`) en draait volledig in je browser. Je Strava-sleutels blijven in je eigen browser en komen nergens anders terecht.

## Stap 1 — Strava API-sleutel aanmaken (eenmalig, gratis)

1. Ga naar https://www.strava.com/settings/api (log in met je Strava-account).
2. Vul in: naam bv. "RunAi", categorie "Training", website mag je eigen URL zijn.
3. Bij **Authorization Callback Domain** vul je het domein in waar de app komt te staan (zie stap 2), bv. `stijnsamyn.github.io` — zonder https:// en zonder pad.
4. Noteer je **Client ID** en **Client Secret**.

## Stap 2 — Online zetten met GitHub Pages (gratis)

1. Maak een account op https://github.com (als je er nog geen hebt).
2. Klik rechtsboven op "+" → **New repository**. Naam: `runai`. Zet op **Public**. Klik Create.
3. Klik "uploading an existing file" en sleep `index.html`, `apple-touch-icon.png` en `icon-512.png` erin. Klik Commit.
4. Ga naar Settings → Pages → bij "Branch" kies `main` en klik Save.
5. Na een minuutje staat je app op: `https://<jouw-gebruikersnaam>.github.io/runai/`

> Vul dat domein (`<jouw-gebruikersnaam>.github.io`) in als Callback Domain in stap 1.3.

## Stap 3 — Op je iPhone

1. Open de URL in Safari.
2. Vul eenmalig je Client ID en Client Secret in en tik "Verbinden met Strava".
3. Deel-knop → **Zet op beginscherm** → je hebt een app-icoon met je schema, statistieken en dagelijkse aanbeveling.

## Bijwerken

Nieuwe versie van `index.html`? Upload het bestand opnieuw in je GitHub-repository (Add file → Upload files → Commit). De site vernieuwt automatisch.

## Problemen?

- **"Strava-login mislukt"**: controleer Client ID/Secret en of het Callback Domain exact overeenkomt met het domein van de URL.
- **Lege pagina na inloggen**: herlaad de pagina één keer.
- Lukt iets niet — vraag het aan Claude in het RunAi-project.
