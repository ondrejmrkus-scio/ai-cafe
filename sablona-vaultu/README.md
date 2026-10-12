# Šablona: pracovní kontext na jednom místě

Tohle je složka, kterou otevřeš v Claude Code (nebo v desktop aplikaci Claude jako projekt). Claude v ní ví, kam jít pro kontext, a načítá jen to, co je pro zadání potřeba. Drží to tři vrstvy:

- `CLAUDE.md`: pravidla, jak se má Claude chovat. Načítají se automaticky na začátku každé konverzace.
- `MEMORY.md`: fakta, která se můžou změnit. `CLAUDE.md` ji řádkem `@MEMORY.md` vkládá do kontextu od první zprávy a Claude do ní zapíše, když řekneš „zapamatuj si".
- `00_Resources/`: dokumenty, které Claude otevře, až když je potřebuje. Který a kdy, to říká tabulka v `CLAUDE.md`.

## Jak začít (asi hodina)

1. Zkopíruj tuhle složku kamkoliv a přejmenuj ji. V Claude Code ji otevři jako pracovní složku.
2. Otevři `CLAUDE.md` a vyplň všechno v hranatých závorkách. Nepiš víc, než je nutné. Další pravidla přidávej, až když ti budou chybět.
3. Do `00_Resources/` dej dva až tři dokumenty, ke kterým se při práci vracíš, a doplň je do tabulky Resources v `CLAUDE.md` i s poznámkou, kdy je číst.
4. Vyzkoušej to: zeptej se na něco, co je v paměti. Pak řekni „zapamatuj si, že…" a podívej se do `MEMORY.md`, co se zapsalo.

## Kam co patří: dva testy

- Předepisuje to chování? Poznáš to podle slov „vždy", „nikdy", „před X udělej Y". Patří to do `CLAUDE.md`.
- Je to fakt, který se může změnit? Kontakt, stav projektu, rozhodnutí a důvod, proč padlo. Patří to do `MEMORY.md`.
- Všechno ostatní je zdroj: dokument v `00_Resources/` a řádek v tabulce.

## Víc projektů v jedné složce

Když vedeš víc projektů, které sdílí kontext (stejní lidé, stejná firma), nezakládej víc složek. Každý projekt dostane podsložku s vlastním `CLAUDE.md` a `MEMORY.md`. Načítají se obě úrovně, nadřazená první. Projektová pravidla upřesňují sdílená. Kde projekt nic neříká, platí sdílené. Ukázka je v `Projekt-ukazka/`.

## Verzuj to

Dej složku do gitu. Když Claude zapíše do paměti něco špatně, dá se to vrátit. A vidíš, co se kdy změnilo.
