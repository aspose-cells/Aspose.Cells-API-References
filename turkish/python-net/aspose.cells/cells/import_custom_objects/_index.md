---
title: import_custom_objects yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 640
url: /tr/python-net/aspose.cells/cells/import_custom_objects/
is_root: false
---
##  import_custom_objects(list, first_row, first_column, options) {#list-int-int-ImportTableOptions}
Özel nesneleri içe aktarır.


###  İadeler

İçe aktarılan toplam satır sayısı.


```python
def import_custom_objects(self, list, first_row, first_column, options):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| list | list | özel nesne|
| first_row | int | İçe aktarılacak ilk hücrenin satır numarası.|
| first_column | int | İçe aktarılacak ilk hücrenin sütun numarası.|
| options | [ImportTableOptions](/cells/tr/python-net/aspose.cells/importtableoptions) | İçe aktarma seçenekleri.|
###  Notlar

Özel nesneler aynı türde olmalıdır.

##  import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number) {#list-list-bool-int-int-int-bool-str-bool}

Özel nesneleri içe aktarır.


###  İadeler

İçe aktarılan toplam satır sayısı.


```python
def import_custom_objects(self, list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| list | list | özel nesne|
| property_names | list | Özellik adları Eğer null ise, nesnenin tüm özelliklerini içe aktaracağız.|
| is_property_name_shown | bool | Özellik adının ilk satıra aktarılıp aktarılmayacağını belirtir.|
| first_row | int | İçe aktarılacak ilk hücrenin satır numarası.|
| first_column | int | İçe aktarılacak ilk hücrenin sütun numarası.|
| row_number | int | İçe aktarılacak satır sayısı.|
| insert_rows | bool | Verileri sığdırmak için fazladan satırların eklenip eklenmediğini gösterir.|
| date_format_string | str | Hücreler için tarih biçimi dizesi.|
| convert_string_to_number | bool | Bu yöntemin dizeyi sayıya dönüştürmeye çalışıp çalışmayacağını gösterir.|
###  Notlar

Özel nesneler aynı türde olmalıdır.


###  Ayrıca bakınız

* modül [aspose.cells](../../)
* sınıf [Cells](/cells/tr/python-net/aspose.cells/cells)
