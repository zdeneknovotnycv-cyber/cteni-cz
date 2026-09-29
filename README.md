# Čtení s kamarádem – verze 2.1.0

Aplikace, ve které dítě čte nahlas a „učitel“ poslouchá, hodnotí a pomáhá.

## Proč to musí být na https

Mikrofon a rozpoznávání řeči prohlížeč povolí jen na zabezpečené adrese (https).
Z HTML souboru uloženého v telefonu **nefungují**. Proto je potřeba složku
jednorázově nahrát na web. Je to zdarma a zabere pár minut.

## Nahrání (GitHub Pages – doporučeno, trvalý odkaz)

1. Na github.com vytvoř nový veřejný repozitář, např. `cteni`.
2. **Add file → Upload files** a přetáhni sem všechny soubory z této složky
   (`index.html`, `manifest.webmanifest`, `sw.js`, `icon-*.png`). Potvrď **Commit**.
3. **Settings → Pages → Branch: main, složka / (root) → Save.**
4. Za minutu až dvě bude aplikace na adrese
   `https://TVOJE-JMENO.github.io/cteni/`.

Rychlá alternativa: https://app.netlify.com/drop – přetáhni celou složku a dostaneš
https odkaz (bez přihlášení po čase zmizí, tak se přihlas a nech si ho).

## Ikona na ploše telefonu

**Android (Chrome):** otevři odkaz → ⋮ → **Nainstalovat aplikaci** (nebo
**Přidat na plochu**). Ikona se objeví mezi aplikacemi.
**iPhone (Safari):** Sdílet → **Přidat na plochu**. Pozor: rozpoznávání řeči na
iPhonu bývá nespolehlivé, hlavně v ikoně na ploše. Nejlépe funguje Android + Chrome.

## První spuštění

1. Klepni na 🎤 a povol mikrofon, až se prohlížeč zeptá.
2. Když něco nefunguje, otevři **🔧 Test** nahoře. Ukáže, co přesně je špatně
   (adresa, mikrofon, rozpoznávání, hlas), a poradí, jak to opravit.
3. Rozpoznávání řeči používá službu Google, takže potřebuje internet.

## Český hlas učitele

Učitel mluví **jen českým hlasem** (angličtinu jsem zakázal). Pokud zařízení český
hlas nemá, učitel jen píše. Android: Nastavení → Systém → Jazyky a zadávání →
Převod textu na řeč → Google → Nainstalovat hlasová data → Čeština.
Špatně vyslovenou slabiku lze opravit v ⚙️ → „Vlastní výslovnost“ (např. `ok=okk;pi=pí`).

## Soukromí

Knihy, pokrok a statistiky se ukládají jen v tomto telefonu (v prohlížeči).
Do rozpoznávání řeči se posílá jen zvuk čtení službě Google (jako u diktování).

## Aktualizace

Nový `index.html` nahraj do repozitáře přes původní soubor. Aplikace se při
příštím spuštění s internetem sama aktualizuje.
