---
title: FormatConditionType uppräkning
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 2100
url: /sv/python-net/aspose.cells/formatconditiontype/
is_root: false
---
##  FormatConditionType uppräkning
Regeltyp för villkorligt format.



Typen FormatConditionType avslöjar följande medlemmar:

###  Fält
| Fält| Beskrivning|
| :- | :- |
| CELL_VALUE | Denna regel för villkorlig formatering jämför ett cellvärde<br/> till ett formelberäknat resultat med en operator.|
| EXPRESSION | Denna villkorliga formateringsregel innehåller en formel till<br/>utvärdera. När formelresultatet är sant är cellen det<br/> markerad.|
| COLOR_SCALE | Denna villkorliga formateringsregel skapar en graderad<br/> färgskala på cellerna.|
| DATA_BAR | Denna regel för villkorlig formatering visar en graderad<br/> datafältet i cellintervallet.|
| ICON_SET | Denna regel för villkorlig formatering tillämpar ikoner på celler<br/>enligt deras värderingar.|
| TOP10 | Denna regel för villkorlig formatering markerar celler vars<br/>värden faller i den övre N eller nedre N-parentesen, som<br/> specificerad.|
| UNIQUE_VALUES | Denna regel för villkorlig formatering framhäver unika<br/> värden i intervallet.|
| DUPLICATE_VALUES | Denna regel för villkorlig formatering markerar duplicerade<br/> värden.|
| CONTAINS_TEXT | Denna regel för villkorlig formatering framhäver celler<br/>som innehåller given text. Motsvarar att använda SEARCH()<br/>arkfunktion för att avgöra om cellen innehåller<br/> texten.|
| NOT_CONTAINS_TEXT | Denna regel för villkorlig formatering framhäver celler som<br/>innehåller inte given text. Motsvarar att använda SEARCH()<br/>arkfunktion för att avgöra om cellen innehåller<br/> texten eller inte.|
| BEGINS_WITH | Denna regel för villkorlig formatering framhäver celler i<br/>intervall som börjar med den givna texten. Ekvivalent med<br/> använda LEFT() arkfunktionen och jämföra värden.|
| ENDS_WITH | Denna regel för villkorlig formatering framhäver celler som slutar<br/>med given text. Motsvarar att använda arket RIGHT().<br/> funktion och jämföra värden.|
| CONTAINS_BLANKS | Denna regel för villkorlig formatering framhäver celler som<br/>är helt tomma. Motsvarar att använda LEN(TRIM()).<br/>Detta betyder att om cellen endast innehåller tecken<br/>som TRIM() skulle ta bort, då anses den vara tom.<br/> En tom cell anses också vara tom.|
| NOT_CONTAINS_BLANKS | Denna regel för villkorlig formatering framhäver celler som<br/>är inte tomma. Motsvarar att använda LEN(TRIM()). Detta<br/>betyder att om cellen bara innehåller tecken som<br/>TRIM() skulle ta bort, då anses den vara tom. En<br/> tom cell anses också vara tom.|
| CONTAINS_ERRORS | Denna regel för villkorlig formatering markerar celler med<br/>formelfel. Motsvarar att använda ISERROR() ark<br/> funktion för att avgöra om det finns ett formelfel.|
| NOT_CONTAINS_ERRORS | Denna regel för villkorlig formatering framhäver celler<br/>utan formelfel. Motsvarar att använda ISERROR()<br/> arkfunktion för att avgöra om det finns ett formelfel.|
| TIME_PERIOD | Denna regel för villkorlig formatering framhäver celler<br/>som innehåller datum inom den angivna tidsperioden. De<br/>cellens underliggande värde utvärderas, därför<br/>cell behöver inte formateras som ett datum<br/>utvärderas. Till exempel med en cell som innehåller<br/>värde 38913 det villkorliga formatet ska tillämpas if<br/> regeln kräver värdet 2006-07-14.|
| ABOVE_AVERAGE | Denna regel för villkorlig formatering framhäver celler som<br/>är över eller under genomsnittet för alla värden i<br/> räckvidd.|



###  Se även
* modul [aspose.cells](..)
