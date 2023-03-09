---
title: set_embedded_object yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 170
url: /tr/python-net/aspose.cells.drawing/oleobject/set_embedded_object/
is_root: false
---
##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label) {#bool-bytes-str-bool-str}
Gömülü nesne verilerini ayarlar.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| link_to_file | bool | Nesnenin dosyaya bağlanıp bağlanmadığını gösterir.True ise, objectData parametresi dikkate alınmaz.|
| object_data | bytes | Gömülü nesne verileri.|
| source_file_name | str | Dosya adı.|
| display_as_icon | bool | Nesnenin bir simge olarak görüntülenip görüntülenmediğini belirtir.<br/> Doğruysa, orijinal görüntü verileri simgeyle kaplanacaktır.|
| label | str | Simge etiketi. Yalnızca displayAsIcon true olduğunda çalışır.|


##  set_embedded_object(link_to_file, object_data, source_file_name, display_as_icon, label, update_icon) {#bool-bytes-str-bool-str-bool}
Gömülü nesne verilerini ayarlar.



```python
def set_embedded_object(self, link_to_file, object_data, source_file_name, display_as_icon, label, update_icon):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| link_to_file | bool | Nesnenin dosyaya bağlanıp bağlanmadığını gösterir.True ise, objectData parametresi dikkate alınmaz.|
| object_data | bytes | Gömülü nesne verileri.|
| source_file_name | str | Dosya adı.|
| display_as_icon | bool | Nesnenin bir simge olarak görüntülenip görüntülenmediğini belirtir.<br/> Doğruysa, orijinal görüntü verileri simgeyle kaplanacaktır.|
| label | str | Simge etiketi. Yalnızca displayAsIcon true olduğunda çalışır.|
| update_icon | bool | Simgenin otomatik olarak güncellenip güncellenmediğini gösterir.|
###  Notlar

Aspose, gömülü tüm dosya simgelerini güncelleyebileceğinden, `update_icon` ile doğru simgeyi yanlış olarak eklemeniz daha iyi olur.


###  Ayrıca bakınız

* modül [aspose.cells.drawing](../../)
* sınıf [OleObject](/cells/tr/python-net/aspose.cells.drawing/oleobject)
