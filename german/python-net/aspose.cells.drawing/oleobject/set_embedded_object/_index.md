---
title: set_embedded_object Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 170
url: /de/python-net/aspose.cells.drawing/oleobject/set_embedded_object/
is_root: false
---
##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label) {#bool-bytes-str-bool-str}
Legt eingebettete Objektdaten fest.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| link_to_file | bool | Gibt an, ob das Objekt mit der Datei verknüpft ist. Wenn wahr, wird der Parameter objectData ignoriert.|
| object_data | bytes | Die eingebetteten Objektdaten.|
| source_file_name | str | Der Dateiname.|
| display_as_icon | bool | Gibt an, ob das Objekt als Symbol angezeigt wird.<br/> Wenn wahr, werden die ursprünglichen Bilddaten durch das Symbol verdeckt.|
| label | str | Das Icon-Label. Funktioniert nur, wenn displayAsIcon auf true gesetzt ist.|


##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label, update_icon) {#bool-bytes-str-bool-str-bool}
Legt eingebettete Objektdaten fest.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label, update_icon):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| link_to_file | bool | Gibt an, ob das Objekt mit der Datei verknüpft ist. Wenn wahr, wird der Parameter objectData ignoriert.|
| object_data | bytes | Die eingebetteten Objektdaten.|
| source_file_name | str | Der Dateiname.|
| display_as_icon | bool | Gibt an, ob das Objekt als Symbol angezeigt wird.<br/> Wenn wahr, werden die ursprünglichen Bilddaten durch das Symbol verdeckt.|
| label | str | Das Icon-Label. Funktioniert nur, wenn displayAsIcon auf true gesetzt ist.|
| update_icon | bool | Gibt an, ob das Symbol automatisch aktualisiert wird.|
###  Bemerkungen

Da Aspose alle Dateisymbole einbetten kann, ist es besser, dass Sie das richtige Symbol mit `update_icon` als falsch hinzufügen können.


###  Siehe auch

* Modul [aspose.cells.drawing](../../)
* Klasse [OleObject](/cells/de/python-net/aspose.cells.drawing/oleobject)
