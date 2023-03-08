---
title: on_circular Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells/abstractcalculationmonitor/on_circular/
is_root: false
---
##  on_circular(circular_cells_data) {#collections.abc.Iterator}
Implementieren Sie diese Methode, um Geschäfte zu machen, wenn Sie Formeln mit Zirkelbezügen berechnen.


###  Kehrt zurück

Ob die Formel-Engine diese Zellen nach diesem Aufruf kreisförmig berechnen muss.
True, damit die Formel-Engine weiterhin Berechnungen für sie durchführt.
False, damit die Formel-Engine diese Zellen einfach als berechnet markiert.


```python
def on_circular(self, circular_cells_data):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| circular_cells_data | collections.abc.Iterator |IEnumerator mit CalculationCell-Elementen, die Zellen darstellen, die<br/> hängen von Zirkelbezügen ab.|
###  Bemerkungen

In der Implementierung kann der Benutzer auch den erwarteten Wert als berechnetes Ergebnis festlegen
für einen Teil/alle dieser Zellen, sodass die Formel-Engine sie nicht rekursiv berechnet.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [AbstractCalculationMonitor](/cells/de/python-net/aspose.cells/abstractcalculationmonitor)
