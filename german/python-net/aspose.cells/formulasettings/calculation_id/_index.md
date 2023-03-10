---
title: calculation_id Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 50
url: /de/python-net/aspose.cells/formulasettings/calculation_id/
is_root: false
---
##  calculation_id Eigentum

Gibt die Version des Berechnungsmoduls an, das zum Berechnen von Werten in der Arbeitsmappe verwendet wird.

###  Bemerkungen

Diese Eigenschaft dient nur zum Speichern der Einstellungen in der resultierenden Tabellenkalkulationsdatei
damit andere Anwendungen (z. B. MS Excel) beim Laden und Bearbeiten der resultierenden Datei entsprechend handeln können.
Im Fall von MS Excel, wenn der Wert dieser Eigenschaft kleiner als die zugeordnete Neuberechnungs-Engine-ID ist
Mit der Anwendung, die die resultierende Datei öffnet, berechnet die Anwendung die Ergebnisse aller Formeln neu
auf dieser Arbeitsmappe unmittelbar nach dem Laden der Datei.
Aus Leistungsgründen für die Anwendungen der meisten Benutzer berechnen wir keine Formeln automatisch in der Arbeitsmappe.
unabhängig davon, welcher Wert für diese Eigenschaft festgelegt wurde.
###  Definition:
```python
@property
def calculation_id(self):
    ...
@calculation_id.setter
def calculation_id(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [FormulaSettings](/cells/de/python-net/aspose.cells/formulasettings)
