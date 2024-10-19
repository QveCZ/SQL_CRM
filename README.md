# SQL_CRM

Zadaní:

Představte si následující situaci. Pracujete pro firmu, která distribuuje produkty vyžadující odbornou montáž a musí sledovat, kteří odběratelé mají vyškolené zaměstnance. Kdo nemá, tomu nelze zboží prodat. Jelikož je nepraktické sledovat toto v Excelu, požádal vás šéf o doplnění CRM systému o nový modul školení.
Z jednání máte k dispozici tyto informace:
CRM systém už obsahuje tabulky pro výrobce, firmu a osobu.
Existuje několik typů školení, každý výrobce má vlastní typ opravňující k odběru zboží.
Jsou i obecná obchodní školení, která neopravňují k odběru žádného zboží.
U typu školení je třeba uchovávat krátký popis (do seznamu všech školení na webu), dlouhý popis pro detail školení a template pro email s instrukcemi, který CRM systém pošle účastníkům den před zahájením školení.
U školení je potřeba znát datum uskutečnění, stav (plánované, uskutečněné, zrušené), typ, místo a účastníky. U každého účastníka je potřeba sledovat, zda se školení zúčastnil a zda úspěšně zvládl závěrečný test.
Každý typ školení má nějakou kapacitu (firma má jen určité množství školících sad, školící místnost též nelze nafouknout), školení nemůže mít více přihlášených zájemců než je kapacita. Nicméně chceme si ukládat případné náhradníky na termín, abychom jim dali vědět, když se někdo odhlásí (stává se často, firmy primárně řeší své zakázky, pak teprve školení).

Vytvořte na základě výše uvedeného datový model. Pokud není něco jasné, ptejte se.
Nakreslete ER digram pro nový modul i s vazbami na výrobce, firmu a osobu.
Pro účely této úlohy reprezentujte výrobce i firmu pouze pomocí id a názvu, osobu pak id, jménem a vazbou na firmu.
Odprezentujte.
Vytvořte tabulky na základě svého diagramu. Nezapomeňte na primární a cizí klíče, zvolte vhodně datové typy.
Naplňte tabulky pomocí příkazu INSERT vhodnými testovacími daty. Je lepší, když testovací data co nejvíce připomínají reálná. Pro následující úlohy budete potřebovat:
Školení odehrávající se alespoň ve třech různých letech, některé naplánované do budoucnosti.
Alespoň tři výrobce (např.: Control4, AMX, Crestron, Savant, Loxone) a pět typů školení.
Alespoň deset firem (např. copy&paste z https://www.control4.cz/partneri/ nebo https://www.loxone.com/cscz/koupit/najit-partnera/).
Alespoň patnáct osob.
Napište SELECT příkaz, který umožní pro danou firmu zjistit, zda je jí možné prodávat zboží daného výrobce (firma má alespoň jednoho proškoleného zaměstnance).
Napište příkaz SELECT stejný jako v předchozím případě, ale s tím rozdílem, že výrobce vyžaduje školení staré maximálně dva roky.
Vypište seznam uskutečněných školení za minulý rok.
Vypište seznam plánovaných školení na tento rok.
Napište příkaz SELECT, který zjistí nejbližší plánované školení.
Napište příkaz SELECT, který zjistí nejbližší plánované školení v daném místě a pro daného výrobce.
Napište příkaz, který ověří, zda je dané školení plné.
Napište příkaz INSERT, který přidá účastníka ke školení.
