# Šablona: pracovní kontext na jednom místě

Složka, kterou otevřete v Claude Code (nebo v desktop aplikaci Claude jako projekt). Claude v ní ví, kam jít pro kontext, a načítá jen to, co je pro zadání potřeba. Drží to tři vrstvy:

- `CLAUDE.md`: pravidla, jak se má AI chovat. Načítá se automaticky na začátku každé konverzace.
- `MEMORY.md`: fakta, která se můžou změnit. AI ji čte na začátku a zapisuje do ní, když řeknete „zapamatuj si".
- `00_Resources/`: dokumenty, do kterých AI jde, až když je potřebuje. Co a kdy číst říká tabulka v `CLAUDE.md`.

## Jak začít (asi hodina)

1. Zkopírujte tuhle složku kamkoliv a přejmenujte ji. V Claude Code ji otevřete jako pracovní složku.
2. Otevřete `CLAUDE.md` a vyplňte věci v hranatých závorkách. Nepište víc, než je nutné. Pravidla přibývají s prací, ne předem.
3. Do `00_Resources/` dejte dva až tři dokumenty, ke kterým se při práci vracíte, a doplňte je do tabulky Resources v `CLAUDE.md` s poznámkou, kdy je číst.
4. Zkuste to: zeptejte se na něco, co je v paměti. Pak řekněte „zapamatuj si, že…" a podívejte se do `MEMORY.md`.

## Kam co patří: dva testy

- Předepisuje to chování? Slova „vždy", „nikdy", „před X udělej Y". Patří do `CLAUDE.md`.
- Je to fakt o světě, který se může změnit? Kontakt, stav projektu, rozhodnutí a proč padlo. Patří do `MEMORY.md`.
- Všechno ostatní je zdroj: dokument v `00_Resources/` a řádek v tabulce.

## Víc projektů v jedné složce

Když vedete víc projektů, které sdílí kontext (stejní lidé, stejná firma), nedělejte víc složek. Každý projekt dostane podsložku s vlastním `CLAUDE.md` a `MEMORY.md`. Načítají se obě úrovně, nadřazená první. Projekt pravidla zužuje, kde mlčí, platí ta sdílená. Ukázka je v `Projekt-ukazka/`.

## Když nemáte Claude Code

V claude.ai založte Projekt. Do instrukcí projektu vložte obsah `CLAUDE.md`, do znalostí projektu nahrajte `MEMORY.md` a dokumenty ze zdrojů. Paměť se v téhle variantě neaktualizuje sama: když padne něco k zapamatování, přepište `MEMORY.md` ručně a nahrajte ji znovu.

## Tip: verzujte to

Složku si dejte do gitu. Paměť se pak dá vrátit, když AI zapíše něco špatně, a vidíte, co se kdy změnilo.
