---
title: freeze_panes yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 120
url: /tr/python-net/aspose.cells/worksheet/freeze_panes/
is_root: false
---
##  freeze_panes(cell_name, freezed_rows, freezed_columns) {#str-int-int}
Çalışma sayfasında belirtilen hücrede bölmeleri dondurur.



```python
def freeze_panes(self, cell_name, freezed_rows, freezed_columns):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| cell_name | str | Cell adı.|
| freezed_rows | int | Üst bölmedeki görünür satır sayısı, satır dizininden fazla olamaz.|
| freezed_columns | int | Sol bölmedeki görünür sütunların sayısı, sütun dizininden fazla olamaz.|
###  Notlar

Satır dizini ve sütun dizini sıfır olamaz. Satır sayısı ve sütun sayısı
ayrıca hepsi sıfır olamaz.

##  freeze_panes(row, column, freezed_rows, freezed_columns) {#int-int-int-int}
Çalışma sayfasında belirtilen hücrede bölmeleri dondurur.



```python
def freeze_panes(self, row, column, freezed_rows, freezed_columns):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| row | int | Satır dizini.|
| column | int | Sütun dizini.|
| freezed_rows | int | Üst bölmedeki görünür satır sayısı, satır dizininden fazla olamaz.|
| freezed_columns | int | Sol bölmedeki görünür sütunların sayısı, sütun dizininden fazla olamaz.|
###  Notlar

Satır dizini ve sütun dizini sıfır olamaz. Satır sayısı ve sütun sayısı
ayrıca hepsi sıfır olamaz.


İlk iki parametre donma konumunu belirtir ve son iki parametre sol üst bölmede donmuş alanı belirtir.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Worksheet](/cells/tr/python-net/aspose.cells/worksheet)
