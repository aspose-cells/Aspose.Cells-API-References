---
title: set_embedded_object metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 170
url: /sv/python-net/aspose.cells.drawing/oleobject/set_embedded_object/
is_root: false
---
##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label) {#bool-bytes-str-bool-str}
Ställer in inbäddade objektdata.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| link_to_file | bool | Anger om objektet länkar till filen. Om sant, ignoreras parametern objectData.|
| object_data | bytes | Data för inbäddade objekt.|
| source_file_name | str | Filnamnet.|
| display_as_icon | bool | Indikerar om objektet visas som en ikon.<br/> Om det är sant kommer den ursprungliga bilddatan att täckas av en ikon.|
| label | str | Ikonetiketten. Fungerar bara när displayAsIcon är sant.|


##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label, update_icon) {#bool-bytes-str-bool-str-bool}
Ställer in inbäddade objektdata.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label, update_icon):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| link_to_file | bool | Anger om objektet länkar till filen. Om sant, ignoreras parametern objectData.|
| object_data | bytes | Data för inbäddade objekt.|
| source_file_name | str | Filnamnet.|
| display_as_icon | bool | Indikerar om objektet visas som en ikon.<br/> Om det är sant kommer den ursprungliga bilddatan att täckas av en ikon.|
| label | str | Ikonetiketten. Fungerar bara när displayAsIcon är sant.|
| update_icon | bool | Indikerar om ikonen uppdateras automatiskt.|
###  Anmärkningar

Eftersom Aspose kan uppdatera inbäddade alla filikoner, så är det bättre att du kan lägga till korrekt ikon med `update_icon` som falsk.


###  Se även

* modul [aspose.cells.drawing](../../)
* klass [OleObject](/cells/sv/python-net/aspose.cells.drawing/oleobject)
