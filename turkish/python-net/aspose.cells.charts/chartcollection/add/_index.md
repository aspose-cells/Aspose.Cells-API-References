---
title: add yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.charts/chartcollection/add/
is_root: false
---
##  add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column) {#ChartType-int-int-int-int}
Koleksiyona bir grafik ekler.


###  İadeler

[Chart](/cells/tr/python-net/aspose.cells.charts/chart) nesne dizini.


```python
def add(self, type, upper_left_row, upper_left_column, lower_right_row, lower_right_column):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| type | [ChartType](/cells/tr/python-net/aspose.cells.charts/charttype) | Grafik tipi|
| upper_left_row | int | Sol üst sıra dizini.|
| upper_left_column | int | Sol üst sütun dizini.|
| lower_right_row | int | Sağ alt sıra dizini|
| lower_right_column | int | Sağ alt sütun dizini|


##  add(type, data_range, top_row, left_column, right_row, bottom_column) {#ChartType-str-int-int-int-int}
Koleksiyona bir grafik ekler.


###  İadeler

[Chart](/cells/tr/python-net/aspose.cells.charts/chart) nesne dizini.


```python
def add(self, type, data_range, top_row, left_column, right_row, bottom_column):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| type | [ChartType](/cells/tr/python-net/aspose.cells.charts/charttype) | Grafik tipi|
| data_range | str | Grafiğin veri aralığını belirtir|
| top_row | int | Sol üst sıra dizini.|
| left_column | int | Sol üst sütun dizini.|
| right_row | int | Sağ alt sıra dizini|
| bottom_column | int | Sağ alt sütun dizini|
###  Notlar

NOT: Bu üye artık kullanılmıyor. Yerine,
lütfen [ChartCollection.add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/tr/python-net/aspose.cells.charts/chartcollection/add) özelliğini kullanın.
 Bu mülk, Mayıs 2022'den itibaren 12 ay sonra kaldırılacaktır.
Aspose yaşamış olabileceğiniz rahatsızlıktan dolayı özür diler.

##  add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#bytes-str-bool-int-int-int-int}
Önceden ayarlanmış şablona sahip bir grafik ekler.


###  İadeler

[Chart](/cells/tr/python-net/aspose.cells.charts/chart) nesne dizini.


```python
def add(self, data, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| data | bytes | Grafik şablonu dosyasının (.crtx) verileri.|
| data_range | str | Grafiğin veri aralığını belirtir|
| is_vertical | bool | Bir dizi hücre değeri aralığından serinin satıra mı yoksa sütuna göre mi çizileceğini belirtir.|
| top_row | int | Sol üst sıra dizini.|
| left_column | int | Sol üst sütun dizini.|
| right_row | int | Sağ alt sıra dizini|
| bottom_column | int | Sağ alt sütun dizini|


##  add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#ChartType-str-bool-int-int-int-int}
Koleksiyona bir grafik ekler.


###  İadeler

[Chart](/cells/tr/python-net/aspose.cells.charts/chart) nesne dizini.


```python
def add(self, type, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| type | [ChartType](/cells/tr/python-net/aspose.cells.charts/charttype) | Grafik tipi|
| data_range | str | Grafiğin veri aralığını belirtir|
| is_vertical | bool | Bir dizi hücre değeri aralığından serinin satıra mı yoksa sütuna göre mi çizileceğini belirtir.|
| top_row | int | Sol üst sıra dizini.|
| left_column | int | Sol üst sütun dizini.|
| right_row | int | Sağ alt sıra dizini|
| bottom_column | int | Sağ alt sütun dizini|



###  Ayrıca bakınız
* modül [aspose.cells.charts](../../)
* sınıf [Chart](/cells/tr/python-net/aspose.cells.charts/chart)
* sınıf [ChartCollection](/cells/tr/python-net/aspose.cells.charts/chartcollection)
