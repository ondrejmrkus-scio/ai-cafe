# Scio OS: Tvůj pracovní kontext na jednom místě

Pamatovat si Claude umí. Horší je to s pořádkem: pravda o projektu je rozházená po dokumentech, chatech a hlavách a v každé nové konverzaci se skládá znovu. Řešení je jedna složka, kde to všechno bydlí, a pár pravidel, která říkají, co se k jakému zadání načte a co zůstane stranou. Na rozvrh se nenačítá spisovka. Do zprávy pro kolegu se načte tvůj tón.

## Tři vrstvy

| Soubor | Co v něm je | Jak se pozná |
| --- | --- | --- |
| `CLAUDE.md` | **Pravidla.** Kdo jsi, jazyk, tón, co dělat vždy a co nikdy, mapa zdrojů. Načítá se samo. | „vždy", „nikdy", „před X udělej Y" |
| `MEMORY.md` | **Fakta.** Lidé, stav projektů, rozhodnutí a proč padla. Čte se na začátku, zapisuje na „zapamatuj si". | fakt, který se může změnit |
| `00_Resources/` | **Zdroje.** Dokumenty, do kterých se jde, až když jsou potřeba. Které a kdy říká tabulka v pravidlech. | všechno ostatní |

## Tři kroky na dnešní odpoledne

1. **Složka a pět řádků pravidel.** `CLAUDE.md`: kdo jsi, jazyk, tón, dvě věci, které nechceš. Víc ne, pravidla přibývají s prací.
2. **Prázdná paměť a jedno pravidlo k ní.** `MEMORY.md` s nadpisy Lidé, Stav projektů, Rozhodnutí. Do pravidel: „Na začátku si přečti MEMORY.md. Když řeknu zapamatuj si, zapiš to tam hned."
3. **Tři dokumenty, ke kterým se vracíš, a mapa k nim.** Do `00_Resources/` a do tabulky v pravidlech s poznámkou, kdy který číst. Tahle tabulka je to, díky čemu Claude ví, kam jít.

Pak to vyzkoušej: zeptej se na něco, co je v paměti. Řekni „zapamatuj si, že…" a podívej se do souboru. Až přibude druhý projekt, dej mu podsložku s vlastním `CLAUDE.md` a `MEMORY.md`.

## Až to poroste

- **Řekni, co nečíst.** Přepisy, staré verze, cizí rozpracovaná práce. Jinak se do každé konverzace načte všechno.
- **Paměť neduplikuje zdroje.** Když je pravda v dokumentu nebo v repu, paměť drží jen odkaz a důvod, proč rozhodnutí padlo.
- **Verzuj to gitem.** Paměť se dá vrátit a vidíte, co se kdy změnilo.
- **Osobní věci zvlášť.** Soukromé věci do jiné složky, ke které pracovní Claude nemá přístup.
- **Automatizace až nakonec.** Agenti, skills a workflows až když základ nějakou dobu žije.

## Všechno na jedné stránce

https://ondrejmrkus-scio.github.io/ai-cafe/ · postup, strom skutečné složky, šablona ke stažení (zip) a tenhle handout
