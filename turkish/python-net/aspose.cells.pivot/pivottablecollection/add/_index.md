---
title: add yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.pivot/pivottablecollection/add/
is_root: false
---
##  add(source_data, dest_cell_name, table_name) {#str-str-str}
PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.


###  İadeler

Yeni eklenen önbellek dizini.


```python
def add(self, source_data, dest_cell_name, table_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| source_data | str | Yeni PivotTable önbelleği için veriler.|
| dest_cell_name | str |PivotTable raporunun hedef aralığının sol üst köşesindeki hücre.|
| table_name | str | Yeni PivotTable raporunun adı.|


##  add(pivot_table, dest_cell_name, table_name) {#PivotTable-str-str}
Koleksiyona başka bir PivotTable'dan yeni bir PivotTable Nesnesi ekler.


###  İadeler

Yeni eklenen PivotTable dizini.


```python
def add(self, pivot_table, dest_cell_name, table_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/tr/python-net/aspose.cells.pivot/pivottable) | Kaynak pivot tablosu.|
| dest_cell_name | str |PivotTable raporunun hedef aralığının sol üst köşesindeki hücre.|
| table_name | str | Yeni PivotTable raporunun adı.|


##  add(source_data, dest_cell_name, table_name, use_same_source) {#str-str-str-bool}
PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.


###  İadeler

Yeni eklenen önbellek dizini.


```python
def add(self, source_data, dest_cell_name, table_name, use_same_source):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| source_data | str | Yeni PivotTable önbelleği için veriler.|
| dest_cell_name | str |PivotTable raporunun hedef aralığının sol üst köşesindeki hücre.|
| table_name | str | Yeni PivotTable raporunun adı.|
| use_same_source | bool | Mevcut başka bir pivot tablonun bu veri kaynağını kullandığında aynı veri kaynağının kullanılıp kullanılmadığını gösterir.<br/> Özellik true ise, bellekten tasarruf sağlayacaktır.|


##  add(source_data, row, column, table_name) {#str-int-int-str}
PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.


###  İadeler

Yeni eklenen önbellek dizini.


```python
def add(self, source_data, row, column, table_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| source_data | str | Yeni PivotTable için veri hücresi aralığı. Örnek: Sheet1!A1:C8|
| row | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır dizini.|
| column | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun dizini.|
| table_name | str | Yeni PivotTable raporunun adı.|


##  add(pivot_table, row, column, table_name) {#PivotTable-int-int-str}
Koleksiyona başka bir PivotTable'dan yeni bir PivotTable Nesnesi ekler.


###  İadeler

Yeni eklenen PivotTable dizini.


```python
def add(self, pivot_table, row, column, table_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/tr/python-net/aspose.cells.pivot/pivottable) | Kaynak pivot tablosu.|
| row | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır dizini.|
| column | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun dizini.|
| table_name | str | Yeni PivotTable raporunun adı.|


##  add(source_data, row, column, table_name, use_same_source) {#str-int-int-str-bool}
PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.


###  İadeler

Yeni eklenen önbellek dizini.


```python
def add(self, source_data, row, column, table_name, use_same_source):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| source_data | str | Yeni PivotTable için veri hücresi aralığı. Örnek: Sheet1!A1:C8|
| row | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır dizini.|
| column | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun dizini.|
| table_name | str | Yeni PivotTable raporunun adı.|
| use_same_source | bool | Mevcut başka bir pivot tablonun bu veri kaynağını kullandığında aynı veri kaynağının kullanılıp kullanılmadığını gösterir.<br/> Özellik true ise, bellekten tasarruf sağlayacaktır.|


##  add(source_data, is_auto_page, page_fields, dest_cell_name, table_name) {#list-bool-PivotPageFields-str-str}
Veri kaynağı olarak birden çok konsolidasyon aralığıyla koleksiyona yeni bir PivotTable Nesnesi ekler.


###  İadeler

Yeni eklenen PivotTable dizini.


```python
def add(self, source_data, is_auto_page, page_fields, dest_cell_name, table_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| source_data | list | {"Sheet1!A1:C8","Sheet2!A1:B8"} gibi çoklu birleştirme aralıkları |
| is_auto_page | bool | İster otomatik tek sayfa alanı oluşturun.<br/>Doğruysa, aşağıdaki pageFields parametresi yok sayılır.|
| page_fields | [PivotPageFields](/cells/tr/python-net/aspose.cells.pivot/pivotpagefields) | Pivot sayfa alanı öğeleri.|
| dest_cell_name | str | destCellName Yeni PivotTable raporunun adı.|
| table_name | str | yeni PivotTable raporunun adı.|


##  add(source_data, is_auto_page, page_fields, row, column, table_name) {#list-bool-PivotPageFields-int-int-str}
Veri kaynağı olarak birden çok konsolidasyon aralığıyla koleksiyona yeni bir PivotTable Nesnesi ekler.


###  İadeler

Yeni eklenen PivotTable dizini.


```python
def add(self, source_data, is_auto_page, page_fields, row, column, table_name):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| source_data | list | {"Sheet1!A1:C8","Sheet2!A1:B8"} gibi çoklu birleştirme aralıkları |
| is_auto_page | bool | İster otomatik tek sayfa alanı oluşturun.<br/> Doğruysa, aşağıdaki pageFields parametresi yok sayılır|
| page_fields | [PivotPageFields](/cells/tr/python-net/aspose.cells.pivot/pivotpagefields) | Pivot sayfa alanı öğeleri.|
| row | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satır dizini.|
| column | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütun dizini.|
| table_name | str | Yeni PivotTable raporunun adı.|



###  Ayrıca bakınız
* modül [aspose.cells.pivot](../../)
* sınıf [PivotTableCollection](/cells/tr/python-net/aspose.cells.pivot/pivottablecollection)
