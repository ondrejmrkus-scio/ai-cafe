# Paměť pro AI ve třech souborech

AI si z konverzace na konverzaci nepamatuje nic. Stačí tři soubory ve složce, kterou otevřete v Claude Code, a pamatuje si všechno, co potřebujete.

## Tři vrstvy

| Soubor | Co v něm je | Jak se pozná |
| --- | --- | --- |
| `CLAUDE.md` | **Pravidla.** Kdo jste, jazyk, tón, co dělat vždy a co nikdy. Načítá se samo na začátku. | „vždy", „nikdy", „před X udělej Y" |
| `MEMORY.md` | **Fakta.** Lidé, stav projektů, rozhodnutí a proč padla. AI ji čte na začátku a zapisuje do ní na „zapamatuj si". | fakt, který se může změnit |
| `00_Resources/` | **Zdroje.** Dokumenty, do kterých se jde, až když jsou potřeba. V pravidlech je tabulka „čti, když…". | všechno ostatní |

## Tři kroky na dnešní odpoledne

1. **Složka a pět řádků pravidel.** Založte složku, v ní `CLAUDE.md`: kdo jste, jazyk, tón, dvě věci, které nechcete. Víc ne, pravidla přibývají s prací.
2. **Prázdná paměť a jedno pravidlo k ní.** `MEMORY.md` s nadpisy Lidé, Stav projektů, Rozhodnutí. Do pravidel: „Na začátku si přečti MEMORY.md. Když řeknu zapamatuj si, zapiš to tam hned."
3. **Tři dokumenty, ke kterým se vracíte.** Do `00_Resources/` a do tabulky v pravidlech s poznámkou, kdy je číst.

Pak to vyzkoušejte: zeptejte se na něco, co je v paměti. Řekněte „zapamatuj si, že…" a podívejte se do souboru.

## Až to poroste

- **Víc projektů v jedné složce.** Když projekty sdílí lidi a kontext, každý dostane podsložku s vlastním `CLAUDE.md` a `MEMORY.md`. Načítají se obě úrovně, nadřazená první. Projekt pravidla zužuje, kde mlčí, platí sdílená.
- **Verzujte to gitem.** Paměť se dá vrátit, když AI zapíše něco špatně, a vidíte, co se kdy změnilo.
- **Osobní věci zvlášť.** Pracovní složka je pro práci. Soukromé věci do jiné složky, ke které pracovní AI nemá přístup.

## Bez Claude Code

V claude.ai založte Projekt. Instrukce projektu = obsah `CLAUDE.md`. Znalosti projektu = `MEMORY.md` a zdroje. Paměť se neaktualizuje sama, při změně soubor přepište a nahrajte znovu.

## Šablona ke stažení

[odkaz doplnit před akcí] · složka s vyplněnými ukázkami všech tří souborů a návodem v `README.md`
