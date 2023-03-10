---
title: on_circular metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells/abstractcalculationmonitor/on_circular/
is_root: false
---
##  on_circular(circular_cells_data) {#collections.abc.Iterator}
Implementera denna metod för att göra affärer när du beräknar formler med cirkulära referenser.


###  Returnerar

Om formelmotorn behöver beräkna dessa celler i cirkulär efter detta samtal.
Sant att låta formelmotorn fortsätta att göra beräkningar åt dem.
Falskt att låta formelmotorn bara markera dessa celler som beräknade.


```python
def on_circular(self, circular_cells_data):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| circular_cells_data | collections.abc.Iterator | IEnumerator med CalculationCell-objekt som representerar celler som<br/> beror på cirkulära referenser.|
###  Anmärkningar

implementeringen kan användaren också ställa in det förväntade värdet som beräknat resultat
för en del/alla av dessa celler så att formelmotorn inte kommer att beräkna dem rekursivt.


###  Se även
* modul [aspose.cells](../../)
* klass [AbstractCalculationMonitor](/cells/sv/python-net/aspose.cells/abstractcalculationmonitor)
