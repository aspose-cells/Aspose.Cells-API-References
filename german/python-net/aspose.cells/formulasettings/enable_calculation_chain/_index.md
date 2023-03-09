---
title: enable_calculation_chain Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 70
url: /de/python-net/aspose.cells/formulasettings/enable_calculation_chain/
is_root: false
---
##  enable_calculation_chain Eigentum

Ob Berechnungskette für Formeln aktivieren.

###  Bemerkungen

Wenn die Arbeitsmappe viele Formeln enthält und der Benutzer sie wiederholt berechnen muss
Wenn Sie nur einen kleinen Teil davon ändern, kann es für die Leistung hilfreich sein, die Berechnungskette zu aktivieren.
Wenn andererseits die Kette aktiviert ist, erfordert die Aufrechterhaltung des Kettenmodells zusätzlichen Speicher.
und es erfordert auch etwas mehr CPU-Zeit für einige andere Operationen wie das Ändern des Zellenwerts oder der Formeln.
Nachdem diese Eigenschaft von false auf true geändert wurde, wird die Berechnungskette analysiert und aufgebaut
zum Zeitpunkt der ersten Berechnung für die Arbeitsmappe, also die benötigte Zeit für die erste Berechnung
kann mehr als normale Berechnung ohne Kette sein.
###  Definition:
```python
@property
def enable_calculation_chain(self):
    ...
@enable_calculation_chain.setter
def enable_calculation_chain(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [FormulaSettings](/cells/de/python-net/aspose.cells/formulasettings)
