# Scio OS: Tvůj pracovní kontext na jednom místě

Pamatovat si Claude umí. Horší je to s pořádkem: to, co o projektu platí, je rozházené po dokumentech, chatech a hlavách a v každé nové konverzaci se skládá znovu. Řešení je jedna složka, kde to všechno je, a pár pravidel o tom, co se k jakému zadání načte a co zůstane stranou.

## Tři vrstvy

| Soubor | Co v něm je | Jak se pozná |
| --- | --- | --- |
| `CLAUDE.md` | **Pravidla.** Kdo jsi, jakým jazykem a tónem chceš psát, co dělat vždy a co nikdy. A mapa zdrojů: který dokument číst a kdy. Načítá se automaticky. | „vždy", „nikdy", „před X udělej Y" |
| `MEMORY.md` | **Fakta.** Lidé, stav projektů, rozhodnutí a proč padla. Claude ji přečte na začátku a zapíše do ní, když řekneš „zapamatuj si". | fakt, který se může změnit |
| `00_Resources/` | **Zdroje.** Dokumenty, které Claude otevře, až když je potřebuje. Který a kdy, to říká tabulka v pravidlech. | všechno ostatní |

## Tři kroky na dnešní odpoledne

1. **Složka a pět řádků pravidel.** Založ složku a v ní `CLAUDE.md`. Napiš do něj, kdo jsi, jakým jazykem a tónem chceš psát a dvě věci, které nechceš. Víc ne. Další pravidla přidávej, až když ti budou chybět.
2. **Prázdná paměť a jedno pravidlo k ní.** Vytvoř `MEMORY.md` s nadpisy Lidé, Stav projektů a Rozhodnutí. Do `CLAUDE.md` přidej pravidlo: „Na začátku si přečti MEMORY.md. Když řeknu zapamatuj si, zapiš to tam hned."
3. **Tři dokumenty, ke kterým se vracíš, a mapa k nim.** Dej je do `00_Resources/` a do `CLAUDE.md` přidej tabulku: který dokument a kdy ho číst. Díky téhle tabulce Claude ví, kam jít.

Pak to vyzkoušej: zeptej se na něco, co je v paměti, řekni „zapamatuj si, že…" a podívej se, co se do souboru zapsalo. Až přibude druhý projekt, dej mu podsložku s vlastním `CLAUDE.md` a `MEMORY.md`.

## Až to poroste

- **Řekni, co nečíst.** Doslovné přepisy, staré verze, rozpracovaná práce někoho jiného. Jinak se do každé konverzace tahá všechno.
- **Paměť neopisuje zdroje.** Když je pravda v dokumentu nebo v repu, paměť drží jen odkaz na něj a důvod, proč rozhodnutí padlo.
- **Verzuj to gitem.** Paměť se dá vrátit a vidíš, co se kdy změnilo.
- **Osobní věci drž zvlášť.** Soukromé věci patří do jiné složky, ke které Claude z pracovní složky nemá přístup.
- **Automatizace až nakonec.** Agenti, skills a workflows až když základ nějakou dobu používáš.

## Všechno na jedné stránce

https://ondrejmrkus-scio.github.io/ai-cafe/ · postup, strom skutečné složky, šablona ke stažení (zip) a tenhle handout
