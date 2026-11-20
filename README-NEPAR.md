# NEPÁR — interaktívny prototyp e-shopu

## Spustenie
Otvorte súbor `index.html` v prehliadači Chrome, Safari, Firefox alebo Edge. Na zobrazenie Google Fonts a ukážkových fotografií potrebujete internet. Aplikácia je samostatný HTML súbor bez zostavovania.

## Čo funguje
- Responzívna úvodná stránka, produkty a filtrovanie dropu.
- Detail produktu s informáciami o materiáli, pôvode a výrobcovi.
- Košík a formulár dopytu na skladové kusy.
- Custom konfigurátor (typ, farba, materiál, veľkosť, strih, rozmery, poznámka, kontakt) a orientačná cena.
- Administrácia **Ateliér**: pridávanie, úprava, mazanie produktov, množstvá, ceny, fotografie cez URL alebo malé nahraté obrázky, úprava dropu, prehľad lokálnych dopytov, stavy dopytov, export/import JSON.
- Dáta sa zachovajú po obnovení stránky v rovnakej prehliadači prostredníctvom `localStorage`.

## Demo admin
Kliknite na **Ateliér** a zadajte kód `NEPAR2027`. Kód je iba demonštračný, nie bezpečnostná ochrana.

## Dôležité obmedzenia
Toto je **lokálny funkčný prototyp**, nie nasadený e-shop. Zákaznícke údaje a produkty sa nesynchronizujú medzi zariadeniami. Dopyty sa ukladajú iba v konkrétnom prehliadači. Ak v Ateliéri nastavíte e-mail, odoslanie dopytu otvorí e-mailového klienta zákazníka s predvyplnenou správou — zákazník ju musí odoslať sám. Nie je tu online databáza, platobná brána, bezpečné prihlasovanie, automatické e-maily, právne dokumenty ani overenie zásob na serveri.

## Pred zverejnením
1. Pripojiť reálnu databázu (napr. Supabase/Postgres) so serverovým API pre produkty, dopyty, skladové množstvá.
2. Implementovať bezpečnú administrátorskú autentifikáciu a role.
3. Naprogramovať serverové vytváranie objednávok, e-mailové potvrdenia a GDPR/privacy pravidlá.
4. Pripojiť platby (napr. Stripe/GoPay) a dopravu, obchodné podmienky a zákonné informácie.
5. Nahradiť všetky demo fotografie, cenové príklady, tvorcov a výroky o pôvode skutočnými údajmi.
6. Testovať mobil, prístupnosť, spam ochranu, dostupnosť a súbežné objednávky.