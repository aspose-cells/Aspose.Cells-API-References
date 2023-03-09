---
title: create_range yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 190
url: /tr/python-net/aspose.cells/cells/create_range/
is_root: false
---
##  create_range(address) {#str}
Aralığın adresinden bir [Range](/cells/tr/python-net/aspose.cells/range) nesnesi oluşturur.


###  İadeler

[Range](/cells/tr/python-net/aspose.cells/range) nesnesi


```python
def create_range(self, address):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| address | str | Aralığın adresi.|


##  create_range(upper_left_cell, lower_right_cell) {#str-str}
Bir dizi hücreden bir [Range](/cells/tr/python-net/aspose.cells/range) nesnesi oluşturur.


###  İadeler

[Range](/cells/tr/python-net/aspose.cells/range) nesnesi


```python
def create_range(self, upper_left_cell, lower_right_cell):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_cell | str | Sol üst hücre adı.|
| lower_right_cell | str | Sağ alt hücre adı.|


##  create_range(first_index, number, is_vertical) {#int-int-bool}
Hücre sıralarından veya hücre sütunlarından bir [Range](/cells/tr/python-net/aspose.cells/range) nesnesi oluşturur.


###  İadeler

Bir [Range](/cells/tr/python-net/aspose.cells/range) nesnesi.


```python
def create_range(self, first_index, number, is_vertical):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| first_index | int | İlk satır dizini veya ilk sütun dizini, sıfır tabanlı.|
| number | int | Bir tabanlı toplam satır veya sütun sayısı.|
| is_vertical | bool | True - Hücre sütunlarından oluşturulan aralık. Yanlış - Hücre sıralarından oluşturulan aralık.|


##  create_range(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Bir dizi hücreden bir [Range](/cells/tr/python-net/aspose.cells/range) nesnesi oluşturur.


###  İadeler

[Range](/cells/tr/python-net/aspose.cells/range) nesnesi


```python
def create_range(self, first_row, first_column, total_rows, total_columns):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| first_row | int | Bu aralığın ilk satırı|
| first_column | int | Bu aralığın ilk sütunu|
| total_rows | int | Satır sayısı|
| total_columns | int | Sütun sayısı|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cells](/cells/tr/python-net/aspose.cells/cells)
* sınıf [Range](/cells/tr/python-net/aspose.cells/range)
