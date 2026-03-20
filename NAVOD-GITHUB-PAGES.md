# CompressionFashion.com — GitHub Pages Deployment
# Návod krok za krokem

## Co budeš potřebovat
- GitHub účet (zdarma na github.com)
- Soubory z této složky (stáhneš níže)
- 20 minut času

---

## KROK 1 — Vytvoř GitHub účet (pokud ještě nemáš)
1. Jdi na https://github.com
2. Klikni "Sign up"
3. Použij email contact@compressionfashion.com

---

## KROK 2 — Vytvoř nový repozitář
1. Po přihlášení klikni zelené tlačítko "New" (vlevo nahoře)
2. Repository name: `compressionfashion-com`
3. Nastav na "Public" (nutné pro free GitHub Pages)
4. Zaškrtni "Add a README file"
5. Klikni "Create repository"

---

## KROK 3 — Nahraj soubory
1. V repozitáři klikni "Add file" → "Upload files"
2. Přetáhni VŠECHNY soubory z této složky:
   - index.html
   - about.html
   - guides.html
   - what-is-compression-fashion.html
   - privacy-policy.html
   - affiliate-disclosure.html
   - style.css
   - robots.txt
   - sitemap.xml
3. Dole napiš commit message: "Initial site launch"
4. Klikni "Commit changes"

---

## KROK 4 — Zapni GitHub Pages
1. V repozitáři klikni "Settings" (záložka nahoře)
2. Vlevo v menu klikni "Pages"
3. Pod "Source" vyber "Deploy from a branch"
4. Branch: "main" / Folder: "/ (root)"
5. Klikni "Save"
6. Počkej 2-3 minuty → web bude live na:
   https://[tvoje-jmeno].github.io/compressionfashion-com/

---

## KROK 5 — Připoj vlastní doménu (po 20. březnu)
Až dorazí compressionfashion.com do GoDaddy:

### V GitHub Pages (Settings → Pages):
1. Do pole "Custom domain" napiš: compressionfashion.com
2. Klikni "Save"
3. Zaškrtni "Enforce HTTPS" (po aktivaci certifikátu)

### V GoDaddy DNS (nebo Cloudflare):
Přidej tyto A záznamy (GitHub Pages IP adresy):
```
Type: A  Name: @  Value: 185.199.108.153
Type: A  Name: @  Value: 185.199.109.153
Type: A  Name: @  Value: 185.199.110.153
Type: A  Name: @  Value: 185.199.111.153
Type: CNAME  Name: www  Value: [tvoje-jmeno].github.io
```

DNS propagace: 30 minut až 24 hodin.

---

## KROK 6 — Google Search Console (hned po aktivaci domény)
1. Jdi na https://search.google.com/search-console
2. Add property → Domain → compressionfashion.com
3. Ověř přes DNS TXT záznam v GoDaddy/Cloudflare
4. Zkontroluj Manual Actions → Security Issues
5. Podej sitemap: https://compressionfashion.com/sitemap.xml

---

## Přidávání dalšího článku (každý měsíc)
1. Zkopíruj soubor what-is-compression-fashion.html
2. Přejmenuj na nový název (např. compression-socks-guide.html)
3. Uprav obsah
4. Nahraj přes GitHub → Add file → Upload files
5. Přidej URL do sitemap.xml
6. Přidej kartu na guides.html a index.html

---

## Soubory webu
| Soubor | Popis |
|--------|-------|
| index.html | Homepage |
| about.html | O webu — klíčové pro Google signál nového majitele |
| guides.html | Přehled článků |
| what-is-compression-fashion.html | První článek (plný obsah + FAQ schema) |
| privacy-policy.html | Povinná stránka |
| affiliate-disclosure.html | Povinná stránka |
| style.css | Všechny styly |
| robots.txt | Povoluje indexaci, ukazuje sitemap |
| sitemap.xml | Mapa webu pro Google |
