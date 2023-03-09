---
title: merge yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 790
url: /tr/python-net/aspose.cells/cells/merge/
is_root: false
---
##  merge(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Belirli bir hücre aralığını tek bir hücrede birleştirir.



```python
def merge(self, first_row, first_column, total_rows, total_columns):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| first_row | int | Bu aralığın ilk satırı (sıfır tabanlı)|
| first_column | int | Bu aralığın ilk sütunu (sıfır tabanlı)|
| total_rows | int | Satır sayısı (bir tabanlı)|
| total_columns | int | Sütun sayısı (bir tabanlı)|
###  Notlar

Aralıktaki sol üst hücrenin adresi aracılığıyla birleştirilmiş hücreye başvurun.

##  merge(first_row, first_column, total_rows, total_columns, merge_conflict) {#int-int-int-int-bool}

Belirli bir hücre aralığını tek bir hücrede birleştirir.



```python
def merge(self, first_row, first_column, total_rows, total_columns, merge_conflict):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| first_row | int | Bu aralığın ilk satırı (sıfır tabanlı)|
| first_column | int | Bu aralığın ilk sütunu (sıfır tabanlı)|
| total_rows | int | Satır sayısı (bir tabanlı)|
| total_columns | int | Sütun sayısı (bir tabanlı)|
| merge_conflict | bool | Birleştirme çakışması birleştirilmiş aralıklar.|
###  Notlar

Aralıktaki sol üst hücrenin adresi aracılığıyla birleştirilmiş hücreye başvurun.
mergeConflict true ise ve birleştirilmiş aralık diğer birleştirilmiş hücrelerle çakışıyorsa,
Diğer birleştirilmiş hücreler otomatik olarak kaldırılacaktır.

##  merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict) {#int-int-int-int-bool-bool}
Belirli bir hücre aralığını tek bir hücrede birleştirir.



```python
def merge(self, first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| first_row | int | Bu aralığın ilk satırı (sıfır tabanlı)|
| first_column | int | Bu aralığın ilk sütunu (sıfır tabanlı)|
| total_rows | int | Satır sayısı (bir tabanlı)|
| total_columns | int | Sütun sayısı (bir tabanlı)|
| check_conflict | bool | Kontrol edilen birleştirilmiş hücrelerin diğer birleştirilmiş hücrelerle kesişip kesişmediğini gösterir|
| merge_conflict | bool | Birleştirme çakışması birleştirilmiş aralıklar.|
###  Notlar

Aralıktaki sol üst hücrenin adresi aracılığıyla birleştirilmiş hücreye başvurun.
mergeConflict true ise ve birleştirilmiş aralık diğer birleştirilmiş hücrelerle çakışıyorsa,
Diğer birleştirilmiş hücreler otomatik olarak kaldırılacaktır.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cells](/cells/tr/python-net/aspose.cells/cells)
