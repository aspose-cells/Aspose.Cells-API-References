---
title: AccessCacheOptions uppräkning
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1740
url: /sv/python-net/aspose.cells/accesscacheoptions/
is_root: false
---
##  AccessCacheOptions uppräkning
Cachealternativ för dataåtkomst. Kan kombineras med |-operatör för flera alternativ tillsammans.



Typen AccessCacheOptions avslöjar följande medlemmar:

###  Fält
| Fält| Beskrivning|
| :- | :- |
| NONE | Inget cache för dataåtkomst.|
| ALL | Tillämpa alla möjliga optimeringar för alla typer av dataåtkomst i arbetsboken.<br/> Alla inställningar och data ska inte ändras under den optimerade åtkomsten.|
| POSITION_AND_SIZE | Tillämpa möjlig optimering för att få objektets (som Shape) position och storlek.<br/>Inställningarna för radhöjd och kolumnbredd ska inte ändras under den optimerade åtkomsten.|
| CELLS_DATA | Tillämpa möjlig optimering för att få cellers värden.<br/>Cells-data (data och inställningar för Cell, rad) bör inte ändras under<br/>den optimerade åtkomsten, inga nya Cell/Row-objekt ska heller skapas (som t.ex.<br/> av [[indexer]](/cells/python-net/aspose.cells/cells/__getitem__/)).|
| CELL_DISPLAY | Tillämpa möjlig optimering för att få visningsrelaterade resultat av<br/>celler ([Cell.display_string_value](/cells/sv/python-net/aspose.cells/cell#display_string_value), [Cell.get_style()](/cells/sv/python-net/aspose.cells/cell/get_style), [Cell.get_display_style()](/cells/sv/python-net/aspose.cells/cell/get_display_style), etc.).<br/>Cells data och stilrelaterade objekt (Cell/rad/kolumnstilar, kolumnbredd etc.) ska inte ändras<br/> under den optimerade åtkomsten.|
| GET_FORMULA | Tillämpa möjlig optimering för att få formler.<br/>Alla data och inställningar som kan påverka formeluttrycket (arbetsbladets namn, namnets text,<br/> tabellens kolumner etc.) bör inte ändras under den optimerade åtkomsten.|
| SET_FORMULA | Tillämpa möjliga optimeringar för att ställa in formler.<br/>Alla data och inställningar som kan påverka formeluttrycket (arbetsbladets namn, namnets text,<br/> tabellens kolumner etc.) bör inte ändras under den optimerade åtkomsten.|
| CALCULATE_FORMULA |Tillämpa möjlig optimering för beräkning av formler.<br/>Cells-data bör inte ändras under den optimerade åtkomsten, inga nya objekt (Cell, rad, etc.)<br/> bör skapas antingen (som av [[indexerare]](/cells/python-net/aspose.cells/cells/__getitem__/)).|
| CONDITIONAL_FORMATTING | Tillämpa möjlig optimering för att få formateringsresultat av villkorliga formateringar.<br/>Alla data och inställningar som kan påverka resultatet av villkorlig formatering (inställningar för<br/> villkorlig formatering, beroende cellvärden etc.) bör inte ändras under den optimerade åtkomsten.|
| VALIDATION | Tillämpa möjlig optimering för att få valideringsresultat.<br/>Alla data och inställningar som kan påverka resultatet av valideringen (inställningar för valideringen,<br/> beroende cellvärden etc.) bör inte ändras under den optimerade åtkomsten.|



###  Anmärkningar

För vissa funktioner kräver åtkomst av stora datamängder många upprepade och komplicerade operationer
som sökning, beräkning, ... etc och de operationerna kommer att ta mycket extra tid.
För vanliga situationer förblir all beroende data oförändrad under åtkomsten, så vissa cacher kan byggas och användas för att
förbättra åtkomstprestandan.
För detta ändamål tillhandahåller vi denna API så att användaren kan specificera vilken typ av dataåtkomstbehov
optimeras med möjlig cachningsmekanism.


Observera att för olika alternativ kan det krävas att olika datauppsättningar är "skrivskyddade".
Och prestanda för att komma åt data beror på många aspekter, användningen av caching mekanism
garanterar inte att prestandan kommer att förbättras.
som att datauppsättningen som ska nås är liten, kan användning av cache orsaka ännu mer tid eftersom
själva cachen kräver också viss extra tid.

###  Se även
* modul [aspose.cells](..)
