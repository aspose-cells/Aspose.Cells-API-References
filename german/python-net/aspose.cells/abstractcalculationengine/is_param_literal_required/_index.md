---
title: is_param_literal_required Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells/abstractcalculationengine/is_param_literal_required/
is_root: false
---
##  is_param_literal_required Eigentum

Gibt an, ob diese Engine während der Berechnung den wörtlichen Text des Parameters benötigt. Der Standardwert ist falsch.

###  Bemerkungen

Wenn dieses benutzerdefinierte Berechnungsmodul den wörtlichen Text des Parameters benötigt, sind weitere Stapel erforderlich, um den wörtlichen Text für Parameter zwischenzuspeichern, und die Methode Calculate() kann rekursiv aufgerufen werden, um den Wert des Parameters zu berechnen.
Normalerweise wird der wörtliche Text nicht zum Berechnen von Formeln benötigt, und diese Methode sollte für die meisten Implementierungen falsch zurückgeben, um eine bessere Leistung zu erzielen.
###  Definition:
```python
@property
def is_param_literal_required(self):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [AbstractCalculationEngine](/cells/de/python-net/aspose.cells/abstractcalculationengine)
