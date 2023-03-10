---
title: ConnectionParameter klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 10
url: /sv/python-net/aspose.cells.externalconnections/connectionparameter/
is_root: false
---
##  ConnectionParameter klass
Anger egenskaper för alla parametrar som används med externa dataanslutningar
Parametrar är giltiga för ODBC och webbfrågor.



Typen ConnectionParameter avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [sql_type](/cells/sv/python-net/aspose.cells.externalconnections/connectionparameter/sql_type) | SQL-datatyp för parametern. Endast giltigt för ODBC-källor.|
| [refresh_on_change](/cells/sv/python-net/aspose.cells.externalconnections/connectionparameter/refresh_on_change) | Flagga som anger om frågan ska uppdateras automatiskt när innehållet i en<br/> cell som ger parametervärdeändringarna. Om det är sant uppdateras externa data<br/> använder det nya parametervärdet varje gång det sker en förändring. Om falsk, extern data<br/> uppdateras endast när användaren begär det, eller någon annan händelse utlöser uppdatering (t.ex. om arbetsboken öppnas).|
| [prompt](/cells/sv/python-net/aspose.cells.externalconnections/connectionparameter/prompt) | Fråga sträng för parametern. Presenteras för kalkylarksanvändaren tillsammans med inmatningsgränssnittet<br/> för att samla in parametervärdet innan extern data uppdateras. Används endast när<br/>parameterType = prompt.|
| [type](/cells/sv/python-net/aspose.cells.externalconnections/connectionparameter/type) | Typ av parameter som används.<br/> Om parameterType=värde, då värdet från boolean, double, integer,<br/> eller sträng kommer att användas. I detta fall förväntas endast en av<br/> {boolean, double, integer, or string} kommer att anges.|
| [name](/cells/sv/python-net/aspose.cells.externalconnections/connectionparameter/name) | Namnet på parametern.|
| [cell_reference](/cells/sv/python-net/aspose.cells.externalconnections/connectionparameter/cell_reference) | Cell referens som anger vilken cells värde som ska användas för frågeparametern. Används endast när parameterType är cell.|
| [value](/cells/sv/python-net/aspose.cells.externalconnections/connectionparameter/value) | Icke-heltals numeriskt värde, heltalsvärde, strängvärde eller booleskt värde<br/> att använda som frågeparameter. Används endast när parameterType är värde.|



###  Se även
* modul [aspose.cells.externalconnections](..)
