# IFDB - TV Serije

Aplikacija za pregled i pretraživanje TV serija, glumaca i epizoda s mogućnošću spremanja omiljenih serija po korisničkom računu. Izgrađena je u Next.js-u i koristi TVmaze API.

## Ključne funkcionalnosti
- Početna lista serija
- Dinamičke rute za detalje serije, glumca i epizode
- Dodavanje i brisanje favorita (privremeno u cookie)
- Stranica /favorites za pregled omiljenih serija
- Prikaz 404 stranice za nepostojeće rute
- Deploy na Vercel (ili vlastiti server)

## Upute za lokalno pokretanje
1. Klonirajte repozitorij:
   ```bash
   git clone https://github.com/gaunterOdimm24/IFDb3.git
   cd IFDB2-main
   ```
2. Instalirajte ovisnosti:
   ```bash
   npm install
   ```
3. Pokrenite razvojni server:
   ```bash
   npm run dev
   ```
   Aplikacija će biti dostupna na [http://localhost:3000](http://localhost:3000).

**Napomena:**
- Za prijavu putem Google računa potrebno je postaviti Google OAuth ključeve u `.env` datoteku:
  - `GOOGLE_CLIENT_ID=...`
  - `GOOGLE_CLIENT_SECRET=...`
- Ako koristite custom domenu, postavite i `NEXT_PUBLIC_SITE_URL` varijablu.

## Build & Deploy
Za produkcijski build pokrenite:
```bash
npm run build
```
Za lokalno testiranje produkcijskog builda:
```bash
npm start
```
Deploy preporučujemo na [Vercel](https://vercel.com/). Nakon deploya, aplikacija će biti dostupna na vašem Vercel URL-u.

## Poznate greške / TODO
- Favoriti se trenutno spremaju u cookie i nisu trajno vezani uz korisnički račun (planira se nadogradnja na bazu podataka)
- Trenutno je podržana samo prijava putem Google računa
- UI nije u potpunosti prilagođen za mobilne uređaje

---
Za pitanja i prijedloge, slobodno se obratite!
