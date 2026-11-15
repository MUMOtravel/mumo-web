# MUMO Travel – moduly pre web

Samostatné moduly pre stránku mumotravel.com (Landingsite). Každý modul je jeden JavaScript súbor,
ktorý si sám načíta svoje štýly a dáta, takže sa nebije so štýlmi Landingsite.

| Súbor | Čo robí |
|---|---|
| `mumo-mapa.js` | Výber výletu s detailnou mapou: skutočné cesty, km a čas jazdy, kreslená dodávka jazdí po trase, prepínač Z Viedne / Z Bratislavy |
| `mumo-asistent.js` | Plávajúci asistent vpravo dole: poradí výlet, ceny a pošle odkaz na rezerváciu |
| `demo.html` | Testovacia stránka s oboma modulmi |

## Vloženie do Landingsite (cez AI chat v editore)

Kódy nižšie používajú bezplatné CDN jsDelivr, ktoré súbory servíruje priamo z tohto repozitára.


**Mapa výletov** – do AI chatu napíšte:

> Pridaj pod sekciu s výletmi novú sekciu na celú šírku stránky a vlož do nej presne tento kód:

```html
<div id="mumo-mapa"></div>
<script src="https://cdn.jsdelivr.net/gh/MUMOtravel/mumo-web@main/mumo-mapa.js" defer></script>
```

**Asistent** – do AI chatu napíšte:

> Pridaj tento skript na všetky stránky webu, pred koniec tela stránky:

```html
<script src="https://cdn.jsdelivr.net/gh/MUMOtravel/mumo-web@main/mumo-asistent.js" defer></script>
```

## Zdroje dát

- Mapa: Natural Earth (public domain)
- Trasy: © OpenStreetMap prispievatelia, výpočet OSRM (ODbL) – uvedené priamo v mape
