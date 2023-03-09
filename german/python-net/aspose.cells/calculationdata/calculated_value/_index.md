---
title: calculated_value Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 50
url: /de/python-net/aspose.cells/calculationdata/calculated_value/
is_root: false
---
##  calculated_value Eigentum

Ruft den berechneten Wert für diese Funktion ab oder legt diesen fest.

###  Bemerkungen

Der Benutzer sollte diese Eigenschaft in seiner benutzerdefinierten Berechnungs-Engine für die Funktionen festlegen, die die Engine unterstützt.
und der festgelegte Wert wird zurückgegeben, wenn diese Eigenschaft später abgerufen wird.
Der eingestellte Wert kann ein beliebiger Wert dieser Objekte sein, die auf Cell(Cell.Wert) eingestellt werden können.
Und es kann auch ein Array solcher Werte oder ein Range, Name, ReferredArea sein.
Wenn Sie diese Eigenschaft vor der Einstellung erhalten, wird die Funktion von der Standardberechnungs-Engine von Aspose.Cells berechnet und der berechnete Wert wird zurückgegeben.
###  Definition:
```python
@property
def calculated_value(self):
    ...
@calculated_value.setter
def calculated_value(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [CalculationData](/cells/de/python-net/aspose.cells/calculationdata)
