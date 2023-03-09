---
title: get_leafs Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 160
url: /de/python-net/aspose.cells/cell/get_leafs/
is_root: false
---
##  get_leafs() {#}
Rufen Sie alle Zellen ab, die direkt auf diese Zelle verweisen und aktualisiert werden müssen, wenn diese Zelle geändert wird.


###  Kehrt zurück

Enumerator zum Aufzählen aller abhängigen Personen (Cell)


```python
def get_leafs(self):
    ...
```


###  Bemerkungen

HINWEIS: Diese Klasse ist jetzt veraltet.
Bitte verwenden Sie Cell.GetDependentsInCalculation(bool), um alle abhängigen Elemente in der Berechnungskette abzurufen.
Diese Property wird 12 Monate später seit Mai 2022 entfernt.
Aspose entschuldigt sich für etwaige Unannehmlichkeiten.

##  get_leafs(recursive) {#bool}
Holen Sie sich alle Zellen, die aktualisiert werden, wenn diese Zelle geändert wird.


###  Kehrt zurück

Enumerator zum Aufzählen aller abhängigen Personen (Cell)


```python
def get_leafs(self, recursive):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| recursive | bool | Ob gibt die Blätter zurück, die nicht direkt auf diese Zelle verweisen<br/> aber Verweis auf andere Blätter dieser Zelle|
###  Bemerkungen

HINWEIS: Diese Klasse ist jetzt veraltet.
Bitte verwenden Sie Cell.GetDependentsInCalculation(bool), um alle abhängigen Elemente in der Berechnungskette abzurufen.
Diese Property wird 12 Monate später seit Mai 2022 entfernt.
Aspose entschuldigt sich für etwaige Unannehmlichkeiten.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Cell](/cells/de/python-net/aspose.cells/cell)
