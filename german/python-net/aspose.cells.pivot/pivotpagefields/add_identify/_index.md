---
title: add_identify Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.pivot/pivotpagefields/add_identify/
is_root: false
---
##  add_identify(range_index, page_item_index) {#int-list}
Legt fest, welche Elementbezeichnung in jedem Seitenfeld verwendet werden soll, um den Datenbereich zu identifizieren.
pageItemIndex.Length muss gleich PageFieldCount sein, also fügen Sie bitte zuerst das Seitenfeld hinzu.



```python
def add_identify(self, range_index, page_item_index):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| range_index | int |Der Konsolidierungsdatenbereichsindex.|
| page_item_index | list | Der Seitenelementindex in jedem Seitenfeld.<br/>pageItemIndex[2] = 1 bedeutet das zweite Element im dritten Feld, das verwendet wird, um diesen Bereich zu identifizieren.<br/> pageItemIndex[1] = -1 bedeutet, dass kein Element im zweiten Feld vorhanden ist, um diesen Bereich zu identifizieren<br/> und MS erstellt automatisch ein "leeres" Element im zweiten Feld, um diesen Bereich zu identifizieren.|



###  Siehe auch
* Modul [aspose.cells.pivot](../../)
* Klasse [PivotPageFields](/cells/de/python-net/aspose.cells.pivot/pivotpagefields)
