---
title: calc_stack_size Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells/calculationoptions/calc_stack_size/
is_root: false
---
##  calc_stack_size Eigentum

Gibt die Stapelgröße für die rekursive Berechnung von Zellen an.

###  Bemerkungen

Wenn im Abhängigkeitsbaum eine große Anzahl von Zellen rekursiv berechnet werden muss,
StackOverflowException kann im Berechnungsprozess verursacht werden.
Wenn dies der Fall ist, sollte der Benutzer einen kleineren Wert für diese Eigenschaft angeben.
Für solche Situationen sollte der Benutzer den richtigen Wert für diese Eigenschaft gemäß den tatsächlichen Formeln und Daten bestimmen.
Zu kleine Werte können zu Leistungseinbußen bei der Formelberechnung führen.
###  Definition:
```python
@property
def calc_stack_size(self):
    ...
@calc_stack_size.setter
def calc_stack_size(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [CalculationOptions](/cells/de/python-net/aspose.cells/calculationoptions)
