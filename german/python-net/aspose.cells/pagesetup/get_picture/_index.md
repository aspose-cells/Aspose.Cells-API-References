---
title: get_picture Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 120
url: /de/python-net/aspose.cells/pagesetup/get_picture/
is_root: false
---
##  get_picture(is_header, section) {#bool-int}
Ruft das [Picture](/cells/de/python-net/aspose.cells.drawing/picture)-Objekt der Kopf-/Fußzeile ab.


###  Kehrt zurück

Gibt das Objekt [Picture](/cells/de/python-net/aspose.cells.drawing/picture) zurück.
Gibt null zurück, wenn kein Bild vorhanden ist.


```python
def get_picture(self, is_header, section):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| is_header | bool | Gibt an, ob es sich in der Kopf- oder Fußzeile befindet.|
| section | int | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt.|


##  get_picture(is_first, is_even, is_header, section) {#bool-bool-bool-int}
Ruft das [Picture](/cells/de/python-net/aspose.cells.drawing/picture)-Objekt der Kopf-/Fußzeile ab.


###  Kehrt zurück

Gibt das Objekt [Picture](/cells/de/python-net/aspose.cells.drawing/picture) zurück.


```python
def get_picture(self, is_first, is_even, is_header, section):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| is_first | bool | Gibt an, ob das Bild der Kopf-/Fußzeile der ersten Seite abgerufen wird.|
| is_even | bool | Gibt an, ob das Bild der Kopf-/Fußzeile einer geraden Seite abgerufen wird.|
| is_header | bool | Gibt an, ob das Bild der Kopf-/Fußzeile abgerufen wird.|
| section | int | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt.|



###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [PageSetup](/cells/de/python-net/aspose.cells/pagesetup)
* Klasse [Picture](/cells/de/python-net/aspose.cells.drawing/picture)
