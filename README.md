
--- 

# 🐍 Snake – Konzolna igra u C (Windows)

Ovo je klasična **Snake** igra implementirana u **C jeziku** za **Windows konzolu**, koristeći `windows.h`, `conio.h` i ASCII grafiku. Igra sadrži meni, bodovanje, živote, pauzu, restart i sistem za čuvanje highscore-ova u fajl.

---

## 🎮 Funkcionalnosti

* ASCII grafički prikaz igre u konzoli
* Kontrola zmije strelicama na tastaturi
* Hrana (****) koja povećava dužinu zmije
* Sistem bodovanja
* Sistem života (3 života)
* Pauziranje igre (`P`)
* Povratak u meni (`M`)
* Restart igre (`R`)
* Čuvanje rezultata u fajl
* Pregled highscore liste
* Zvučni efekti (`Beep`)
* Unos imena igrača
* Glavni meni sa navigacijom

---

## 🕹️ Kontrole

| Taster  | Akcija            |
| ------- | ----------------- |
| ⬆ ⬇ ⬅ ➡ | Kretanje zmije    |
| `P`     | Pauza / nastavak  |
| `R`     | Restart igre      |
| `M`     | Povratak u meni   |
| `Q`     | Izlaz iz programa |
| `ENTER` | Potvrda u meniju  |

---

## 🧠 Pravila igre

* Zmija se pomjera konstantno u izabranom smjeru
* Jedenjem hrane:

  * zmija raste
  * score se povećava
* Sudar sa zidom:

  * gubi se jedan život
  * zmija se resetuje
* Sudar sa sopstvenim tijelom:

  * kraj igre
  * rezultat se upisuje u fajl
* Kada životi padnu na 0:

  * igra se završava
  * povratak u meni

---

## 📂 Highscore sistem

Rezultati se čuvaju u tekstualni fajl:

```
score.txt
```

Svaki zapis sadrži:

* ime igrača
* score
* trajanje igre
* preostale živote
* razlog završetka igre

Primjer zapisa:

```
DarkPrince*/imelaptopa/* | Score: 0023 | Time: 45 sec | Lives left: 1 | Reason: Wall collision
```

---

## 🛠️ Tehnički detalji

* Jezik: **C**

* Platforma: **Windows**

* Biblioteke:

  * `stdio.h`
  * `stdlib.h`
  * `conio.h`
  * `windows.h`
  * `time.h`
  * `string.h`

* Dimenzije igrališta:

  * Širina: `40`
  * Visina: `20`

* Maksimalna dužina zmije: `1000`

---

## ⚙️ Kompajliranje (Visual Studio)

1. Kreirati **Console Application**
2. Kopirati kod u `.c` fajl
3. Build & Run (x64 ili Win32)
4. Pokrenuti iz konzole

⚠️ Program koristi **Windows-specifične funkcije** (`Beep`, `SetConsoleCursorPosition`) i neće raditi na Linux/Mac sistemima bez izmjena.

---

## 🧩 Struktura koda

* **Snake logika** – kretanje, rast, sudari
* **Crtanje igre** – ASCII prikaz sa bojama
* **Input sistem** – neblokirajući unos
* **Meni sistem**
* **Highscore sistem**
* **Zvučni efekti**

---

## 🚀 Moguća poboljšanja

* Različiti nivoi težine
* Dinamička brzina zmije
* Prepreke na mapi
* Sortirana highscore lista
* Multiplayer mod
* Grafička verzija (SDL / SFML)

---

## 👤 Autor

**Ime:**Josip Polić
**Projekat:** Snake – konzolna igra
**Jezik:** C
**Godina:** 2025

---
