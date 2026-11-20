# Luxusní pera – koncept nového e-shopu

Statický frontend (HTML + CSS + vanilla JS, bez buildu) pro luxusni-pera.cz, vizuálně inspirovaný patike.ch – stejný designový jazyk jako předchozí koncepty (tmavý rám, zaoblené plochy, plovoucí pill menu, obří „ghost“ nápisy, carousel s výřezy produktů, pozadí se přebarvuje podle barvy pera).

**Jde o neoficiální návrh** – stránka má trvalý pruh „KONCEPT“, vodoznak a `noindex`.

## Co umí
- **Katalog** – 1 782 produktů v 9 kategoriích (plnicí, kuličková pera, rollery, dárkové sady podle značek; diáře, náplně, kaligrafie, kancelář). Velké podkategorie omezené na 60 produktů.
- Barva stránky podle parametru „Barva těla“, carousel z výřezů per postavených na výšku.

## Spuštění lokálně
```bash
cd luxusnipera && python3 -m http.server 8000   # http://localhost:8000
```

## Nasazení
Settings → Pages → Source: **GitHub Actions**, pak Actions → Run workflow. Kořenový `index.html` přesměruje do `luxusnipera/`.

## Co ještě chybí do ostrého provozu
- Platby, sklad a objednávky v reálném čase – ceny jsou snímek z 20. 11. 2026, objednávka zatím odchází e-mailem (mailto).
- Objednávka gravírování (text rytiny) – v ostré verzi jako pole v detailu produktu.
