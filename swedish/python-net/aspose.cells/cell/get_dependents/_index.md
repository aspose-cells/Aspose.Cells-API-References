---
title: get_dependents metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 90
url: /sv/python-net/aspose.cells/cell/get_dependents/
is_root: false
---
##  get_dependents(is_all) {#bool}
Hämta alla celler vars formel refererar till den här cellen direkt.



```python
def get_dependents(self, is_all):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| is_all | bool | Anger om kontrollera formler i andra kalkylblad|
###  Anmärkningar

* Om en referens som innehåller denna cell visas i en cells formel, kommer den cellen att tas som

beroende av denna cell, oavsett referens eller denna cell används eller inte under beräkningen.
Till exempel, även om cell A2 i formeln "=OM(TRUE,A1,A2)" inte används vid beräkning,
denna formel anses fortfarande vara beroende av A2.
För att få de formler vars beräknade resultat beror på den här cellen, använd [Cell.get_dependents_in_calculation(recursive)](/cells/sv/python-net/aspose.cells/cell/get_dependents_in_calculation). När du spårar beroende för en cell kommer alla formler i arbetsboken eller kalkylbladet att analyseras och kontrolleras.
Så det är en tidskrävande process. Om användaren behöver spåra anhöriga för många celler, kommer denna metod att göra det
orsaka dålig prestanda. För prestandaövervägande bör användaren använda [Cell.get_dependents_in_calculation(recursive)](/cells/sv/python-net/aspose.cells/cell/get_dependents_in_calculation) istället.
Eller så kan användaren samla in prejudikatkarta över alla celler med [Cell.get_precedents()](/cells/sv/python-net/aspose.cells/cell/get_precedents) först,
och bygg sedan anhörigkartan enligt prejudikatkartan.

* Om en referens som innehåller denna cell visas i en cells formel, kommer den cellen att tas som
beroende av denna cell, oavsett referens eller denna cell används eller inte under beräkningen.
Till exempel, även om cell A2 i formeln "=OM(TRUE,A1,A2)" inte används vid beräkning,
denna formel anses fortfarande vara beroende av A2.
För att få de formler vars beräknade resultat beror på den här cellen, använd [Cell.get_dependents_in_calculation(recursive)](/cells/sv/python-net/aspose.cells/cell/get_dependents_in_calculation). När du spårar beroende för en cell kommer alla formler i arbetsboken eller kalkylbladet att analyseras och kontrolleras.
Så det är en tidskrävande process. Om användaren behöver spåra anhöriga för många celler, kommer denna metod att göra det
orsaka dålig prestanda. För prestandaövervägande bör användaren använda [Cell.get_dependents_in_calculation(recursive)](/cells/sv/python-net/aspose.cells/cell/get_dependents_in_calculation) istället.
Eller så kan användaren samla in prejudikatkarta över alla celler med [Cell.get_precedents()](/cells/sv/python-net/aspose.cells/cell/get_precedents) först,
och bygg sedan anhörigkartan enligt prejudikatkartan.

* Om en referens som innehåller denna cell visas i en cells formel, kommer den cellen att tas som
beroende av denna cell, oavsett referens eller denna cell används eller inte under beräkningen.
Till exempel, även om cell A2 i formeln "=OM(TRUE,A1,A2)" inte används vid beräkning,
denna formel anses fortfarande vara beroende av A2.
För att få de formler vars beräknade resultat beror på den här cellen, använd [Cell.get_dependents_in_calculation(recursive)](/cells/sv/python-net/aspose.cells/cell/get_dependents_in_calculation). När du spårar beroende för en cell kommer alla formler i arbetsboken eller kalkylbladet att analyseras och kontrolleras.
Så det är en tidskrävande process. Om användaren behöver spåra anhöriga för många celler, kommer denna metod att göra det
orsaka dålig prestanda. För prestandaövervägande bör användaren använda [Cell.get_dependents_in_calculation(recursive)](/cells/sv/python-net/aspose.cells/cell/get_dependents_in_calculation) istället.
Eller så kan användaren samla in prejudikatkarta över alla celler med [Cell.get_precedents()](/cells/sv/python-net/aspose.cells/cell/get_precedents) först,
och bygg sedan anhörigkartan enligt prejudikatkartan.
###  Exempel

```python
from aspose.cells import Workbook

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2"
cells.get("A2").formula = "=IF(TRUE,B2,B1)"
dependents = cells.get("B1").get_dependents(True)
for i in range(len(dependents)):
    print(dependents[i].name)

```



###  Se även
* modul [aspose.cells](../../)
* klass [Cell](/cells/sv/python-net/aspose.cells/cell)
