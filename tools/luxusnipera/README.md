# Aktualizace dat
```bash
python3 tools/luxusnipera/fetch_pages.py urls.txt raw/pages                 # šetrné stažení (4 paralelně, cache)
python3 tools/luxusnipera/parse_shop.py jsonld raw/pages raw/parsed.json     # parsování
python3 tools/luxusnipera/build_catalog.py raw/parsed.json luxusnipera tools/luxusnipera/config.json
HERO_ROTATE=1 python3 tools/luxusnipera/make_hero.py luxusnipera <id produktu> ... # výřezy per (otočené na výšku)
```
Potřeba: Python 3, Pillow, BeautifulSoup4, lxml, curl.
