---
title: get_dependents Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 90
url: /de/python-net/aspose.cells/cell/get_dependents/
is_root: false
---
##  get_dependents(is_all) {#bool}
Holen Sie sich alle Zellen, deren Formel direkt auf diese Zelle verweist.



```python
def get_dependents(self, is_all):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| is_all | bool | Gibt an, ob Formeln in anderen Arbeitsblättern überprüft werden|
###  Bemerkungen

* Wenn ein Verweis, der diese Zelle enthält, in der Formel einer Zelle erscheint, wird diese Zelle als angenommen

abhängig von dieser Zelle, unabhängig davon, ob die Referenz oder diese Zelle während der Berechnung verwendet wird oder nicht.
Obwohl beispielsweise die Zelle A2 in der Formel "=IF(TRUE,A1,A2)" während der Berechnung nicht verwendet wird,
Diese Formel wird immer noch als von A2 abhängig angesehen.
Um die Formeln zu erhalten, deren berechnete Ergebnisse von dieser Zelle abhängen, verwenden Sie bitte [Cell.get_dependents_in_calculation(recursive)](/cells/de/python-net/aspose.cells/cell/get_dependents_in_calculation). Wenn Sie abhängige Elemente für eine Zelle verfolgen, werden alle Formeln in der Arbeitsmappe oder dem Arbeitsblatt analysiert und überprüft.
Es ist also ein zeitaufwändiger Prozess.Wenn Benutzer Abhängigkeiten für viele Zellen verfolgen müssen, wird diese Methode verwendet
kann zu schlechter Leistung führen. Aus Leistungsgründen sollte der Benutzer stattdessen [Cell.get_dependents_in_calculation(recursive)](/cells/de/python-net/aspose.cells/cell/get_dependents_in_calculation) verwenden.
Oder der Benutzer kann zuerst eine Präzedenzfallkarte aller Zellen bis [Cell.get_precedents()](/cells/de/python-net/aspose.cells/cell/get_precedents) sammeln,
und erstellen Sie dann die Abhängigkeitskarte gemäß der Präzedenzfallkarte.

* Wenn ein Verweis, der diese Zelle enthält, in der Formel einer Zelle erscheint, wird diese Zelle als angenommen
abhängig von dieser Zelle, unabhängig davon, ob die Referenz oder diese Zelle während der Berechnung verwendet wird oder nicht.
Obwohl beispielsweise die Zelle A2 in der Formel "=IF(TRUE,A1,A2)" während der Berechnung nicht verwendet wird,
Diese Formel wird immer noch als von A2 abhängig angesehen.
Um die Formeln zu erhalten, deren berechnete Ergebnisse von dieser Zelle abhängen, verwenden Sie bitte [Cell.get_dependents_in_calculation(recursive)](/cells/de/python-net/aspose.cells/cell/get_dependents_in_calculation). Wenn Sie abhängige Elemente für eine Zelle verfolgen, werden alle Formeln in der Arbeitsmappe oder dem Arbeitsblatt analysiert und überprüft.
Es ist also ein zeitaufwändiger Prozess.Wenn Benutzer Abhängigkeiten für viele Zellen verfolgen müssen, wird diese Methode verwendet
kann zu schlechter Leistung führen. Aus Leistungsgründen sollte der Benutzer stattdessen [Cell.get_dependents_in_calculation(recursive)](/cells/de/python-net/aspose.cells/cell/get_dependents_in_calculation) verwenden.
Oder der Benutzer kann zuerst eine Präzedenzfallkarte aller Zellen bis [Cell.get_precedents()](/cells/de/python-net/aspose.cells/cell/get_precedents) sammeln,
und erstellen Sie dann die Abhängigkeitskarte gemäß der Präzedenzfallkarte.

* Wenn ein Verweis, der diese Zelle enthält, in der Formel einer Zelle erscheint, wird diese Zelle als angenommen
abhängig von dieser Zelle, unabhängig davon, ob die Referenz oder diese Zelle während der Berechnung verwendet wird oder nicht.
Obwohl beispielsweise die Zelle A2 in der Formel "=IF(TRUE,A1,A2)" während der Berechnung nicht verwendet wird,
Diese Formel wird immer noch als von A2 abhängig angesehen.
Um die Formeln zu erhalten, deren berechnete Ergebnisse von dieser Zelle abhängen, verwenden Sie bitte [Cell.get_dependents_in_calculation(recursive)](/cells/de/python-net/aspose.cells/cell/get_dependents_in_calculation). Wenn Sie abhängige Elemente für eine Zelle verfolgen, werden alle Formeln in der Arbeitsmappe oder dem Arbeitsblatt analysiert und überprüft.
Es ist also ein zeitaufwändiger Prozess.Wenn Benutzer Abhängigkeiten für viele Zellen verfolgen müssen, wird diese Methode verwendet
kann zu schlechter Leistung führen. Aus Leistungsgründen sollte der Benutzer stattdessen [Cell.get_dependents_in_calculation(recursive)](/cells/de/python-net/aspose.cells/cell/get_dependents_in_calculation) verwenden.
Oder der Benutzer kann zuerst eine Präzedenzfallkarte aller Zellen bis [Cell.get_precedents()](/cells/de/python-net/aspose.cells/cell/get_precedents) sammeln,
und erstellen Sie dann die Abhängigkeitskarte gemäß der Präzedenzfallkarte.
###  Beispiele

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



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
