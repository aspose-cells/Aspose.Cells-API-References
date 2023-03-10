---
title: calculated_value fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 50
url: /sv/python-net/aspose.cells/calculationdata/calculated_value/
is_root: false
---
##  calculated_value fastighet

Hämtar eller ställer in det beräknade värdet för denna funktion.

###  Anmärkningar

Användaren bör ställa in den här egenskapen i sin anpassade beräkningsmotor för de funktioner som motorn stöder,
och det inställda värdet kommer att returneras när du får den här egenskapen senare.
Det inställda värdet kan vara vilket värde som helst av de objekt som kan ställas in på ett Cell(Cell.Value).
Och det kan också vara en rad med sådana värden, eller ett intervall, ett namn, ett refererat område.
Om du får den här egenskapen före inställning kommer funktionen att beräknas av standardberäkningsmotorn Aspose.Cells och det beräknade värdet kommer att returneras.
###  Definition:
```python
@property
def calculated_value(self):
    ...
@calculated_value.setter
def calculated_value(self, value):
    ...
```

###  Se även
* modul [aspose.cells](../../)
* klass [CalculationData](/cells/sv/python-net/aspose.cells/calculationdata)
