# Scio OS: Tvůj pracovní kontext na jednom místě

Claude si pamatovat umí. Co mu chybí, je pořádek: kde je pravda o kterém projektu, co platí vždycky a co se minulý týden změnilo. Řešení je jedna složka, kde to všechno je, a pár pravidel, která říkají, co se kdy načte. Do práce na rozvrhu se nenačítá spisovka. Do textu pro kolegu se načte váš tón.

## O co jde

- **Všechno na jednom místě.** Projekty, které sdílí lidi a rozhodnutí, bydlí v jedné složce jako podsložky. Kontext se neopisuje, sdílí se.
- **Ví, kam jít.** Na začátku se načtou pravidla a paměť. V pravidlech je mapa „čti, když…", která říká, kde je pravda o čem. Zdroje se otevírají, až když jsou na zadání potřeba.
- **Načte jen to, co je relevantní.** Pravidla jsou ve vrstvách: sdílená pro celou složku, užší pro projekt. Co k zadání nepatří, zůstává stranou, i když je ve složce.

## Tři vrstvy

| Soubor | Co v něm je | Jak se pozná |
| --- | --- | --- |
| `CLAUDE.md` | **Pravidla.** Kdo jste, jazyk, tón, co dělat vždy a co nikdy, mapa zdrojů. Načítá se samo. | „vždy", „nikdy", „před X udělej Y" |
| `MEMORY.md` | **Fakta.** Lidé, stav projektů, rozhodnutí a proč padla. Čte se na začátku, zapisuje na „zapamatuj si". | fakt, který se může změnit |
| `00_Resources/` | **Zdroje.** Dokumenty, do kterých se jde, až když jsou potřeba. Které a kdy říká tabulka v pravidlech. | všechno ostatní |

## Tři kroky na dnešní odpoledne

1. **Složka a pět řádků pravidel.** `CLAUDE.md`: kdo jste, jazyk, tón, dvě věci, které nechcete. Víc ne, pravidla přibývají s prací.
2. **Prázdná paměť a jedno pravidlo k ní.** `MEMORY.md` s nadpisy Lidé, Stav projektů, Rozhodnutí. Do pravidel: „Na začátku si přečti MEMORY.md. Když řeknu zapamatuj si, zapiš to tam hned."
3. **Tři dokumenty, ke kterým se vracíte, a mapa k nim.** Do `00_Resources/` a do tabulky v pravidlech s poznámkou, kdy který číst. Tahle tabulka je to, díky čemu Claude ví, kam jít.

Pak to vyzkoušejte: zeptejte se na něco, co je v paměti. Řekněte „zapamatuj si, že…" a podívejte se do souboru. Až přibude druhý projekt, dejte mu podsložku s vlastním `CLAUDE.md` a `MEMORY.md`.

## Až to poroste

- **Řekněte, co nečíst.** Přepisy, staré verze, cizí rozpracovaná práce. Jinak se do každé konverzace načte všechno.
- **Paměť neduplikuje zdroje.** Když je pravda v dokumentu nebo v repu, paměť drží jen odkaz a důvod, proč rozhodnutí padlo.
- **Verzujte to gitem.** Paměť se dá vrátit a vidíte, co se kdy změnilo.
- **Osobní věci zvlášť.** Soukromé věci do jiné složky, ke které pracovní Claude nemá přístup.
- **Automatizace až nakonec.** Agenti, skills a workflows až když základ nějakou dobu žije.

## Bez Claude Code

V claude.ai založte Projekt. Instrukce projektu = obsah `CLAUDE.md`. Znalosti projektu = `MEMORY.md` a zdroje. Paměť se neaktualizuje sama, při změně soubor přepište a nahrajte znovu.

## Všechno na jedné stránce

https://ondrejmrkus-scio.github.io/ai-cafe/ · postup, strom skutečné složky, šablona ke stažení (zip) a tenhle handout
