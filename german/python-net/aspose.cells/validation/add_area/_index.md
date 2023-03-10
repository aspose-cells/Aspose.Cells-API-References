---
title: add_area Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells/validation/add_area/
is_root: false
---
##  add_area(cell_area) {#CellArea}
Wendet die Validierung auf den Bereich an.



```python
def add_area(self, cell_area):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| cell_area | [CellArea](/cells/de/python-net/aspose.cells/cellarea) | Das Gebiet.|
###  Bemerkungen

Es entspricht der Verwendung von [Validation.add_area(cell_area)](/cells/de/python-net/aspose.cells/validation/add_area)
mit Überprüfung von Schnittpunkt und Kante.

##  add_area(cell_area, check_intersection, check_edge) {#CellArea-bool-bool}
Wendet die Validierung auf den Bereich an.



```python
def add_area(self, cell_area, check_intersection, check_edge):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| cell_area | [CellArea](/cells/de/python-net/aspose.cells/cellarea) | Das Gebiet.|
| check_intersection | bool | Ob die Schnittmenge eines bestimmten Bereichs mit den Bereichen bestehender Validierungen überprüft wird.<br/>Wenn eine Validierung in einem bestimmten Bereich (oder einem Teil davon) angewendet wurde,<br/>dann sollte die vorhandene Validierung zunächst aus dem angegebenen Bereich entfernt werden.<br/>Andernfalls können die generierten Validierungen beschädigt werden.<br/>Wenn der Benutzer sicher ist, dass der hinzugefügte Bereich keinen bestehenden Bereich schneidet,<br/> Dieser Parameter kann aus Leistungsgründen auf „false“ gesetzt werden.|
| check_edge | bool | Ob Sie den Rand der angewendeten Bereiche dieser Validierung überprüfen.<br/>Die internen Einstellungen der Validierung hängen von dem oberen linken der angewendeten Bereiche ab,<br/>Wenn also der angegebene Bereich der neue obere linke Bereich der angewendeten Bereiche wird,<br/>Die internen Einstellungen sollten geändert und neu erstellt werden, da es sonst zu unerwarteten Ergebnissen kommen kann.<br/>Wenn der Benutzer sicher ist, dass der hinzugefügte Bereich nicht der obere linke ist,<br/> Dieser Parameter kann aus Leistungsgründen auf „false“ gesetzt werden.|
###  Bemerkungen

Bei dieser Methode entfernen wir alle alten Validierungen in einem bestimmten Bereich.
Für den oberen linken der angewandten Bereiche von Validation ist zunächst die StartRow am kleinsten,
zweitens ist seine Startspalte die kleinste jener Bereiche, die die gleiche kleinste Startzeile haben.


###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Validation](/cells/de/python-net/aspose.cells/validation)
