---
title: SeriesCollection sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 240
url: /tr/python-net/aspose.cells.charts/seriescollection/
is_root: false
---
##  SeriesCollection sınıfı
[Series](/cells/tr/python-net/aspose.cells.charts/series) nesne koleksiyonunu kapsüller.



SeriesCollection türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [category_data](/cells/tr/python-net/aspose.cells.charts/seriescollection/category_data) | Eksen değerleri kategorisinin aralığını alır veya ayarlar.<br/> Bir hücre aralığı olabilir ("d1:e10" gibi),<br/> veya bir değer dizisi ("{2,6,8,10}" gibi).|
| [second_category_data](/cells/tr/python-net/aspose.cells.charts/seriescollection/second_category_data) | İkinci kategori Eksen değerlerinin aralığını alır veya ayarlar.<br/> Bir hücre aralığı olabilir ("d1:e10" gibi),<br/> veya bir değer dizisi ("{2,6,8,10}" gibi).<br/> Yalnızca bazı ASeries'ler ikinci eksende çizildiğinde etki eder.|
| [is_color_varied](/cells/tr/python-net/aspose.cells.charts/seriescollection/is_color_varied) | Noktaların renginin değişip değişmediğini temsil eder.|
| [capacity](/cells/tr/python-net/aspose.cells.charts/seriescollection/capacity) | Dizi listesinin içerebileceği öğe sayısını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add(area, is_vertical)](/cells/tr/python-net/aspose.cells.charts/seriescollection/add/#str-bool) | [SeriesCollection](/cells/tr/python-net/aspose.cells.charts/seriescollection) koleksiyonunu bir grafiğe ekler.|
| [add(area, is_vertical, check_labels)](/cells/tr/python-net/aspose.cells.charts/seriescollection/add/#str-bool-bool) | [SeriesCollection](/cells/tr/python-net/aspose.cells.charts/seriescollection) koleksiyonunu bir grafiğe ekler.|
| [copy_to(array)](/cells/tr/python-net/aspose.cells.charts/seriescollection/copy_to/#list) | Hedef dizi listesinin başından başlayarak tüm dizi listesini uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [copy_to(index, array, array_index, count)](/cells/tr/python-net/aspose.cells.charts/seriescollection/copy_to/#int-list-int-int) |Dizi listesindeki bir dizi öğeyi, hedef dizi listesinin belirtilen dizininden başlayarak uyumlu bir tek boyutlu dizi listesine kopyalar.|
| [index_of(item, index)](/cells/tr/python-net/aspose.cells.charts/seriescollection/index_of/#Series-int) | Belirtilen nesneyi arar ve belirtilen dizinden son öğeye uzanan dizi listesindeki öğelerin aralığındaki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [index_of(item, index, count)](/cells/tr/python-net/aspose.cells.charts/seriescollection/index_of/#Series-int-int) | Belirtilen nesneyi arar ve belirtilen dizinde başlayan ve belirtilen sayıda öğe içeren dizi listesindeki öğe aralığı içindeki ilk oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item)](/cells/tr/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series) | Belirtilen nesneyi arar ve tüm dizi listesindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index)](/cells/tr/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series-int) | Belirtilen nesneyi arar ve ilk öğeden belirtilen dizine kadar uzanan dizi listesindeki öğe aralığı içindeki son oluşumun sıfır tabanlı dizinini döndürür.|
| [last_index_of(item, index, count)](/cells/tr/python-net/aspose.cells.charts/seriescollection/last_index_of/#Series-int-int) |Belirtilen nesneyi arar ve belirtilen sayıda öğeyi içeren ve belirtilen dizinde biten dizi listesindeki öğe aralığındaki son oluşumun sıfır tabanlı dizinini döndürür.|
| [get_series_by_order(order)](/cells/tr/python-net/aspose.cells.charts/seriescollection/get_series_by_order/#int) | [Series](/cells/tr/python-net/aspose.cells.charts/series) öğesini sırayla alır.|
| [change_series_order(source_index, dest_index)](/cells/tr/python-net/aspose.cells.charts/seriescollection/change_series_order/#int-int) | İki dizinin sıralamasını doğrudan değiştirir.|
| [set_series_names(start_index, area, is_vertical)](/cells/tr/python-net/aspose.cells.charts/seriescollection/set_series_names/#int-str-bool) | Grafikteki tüm serilerin adını ayarlar.|
| [add_r1c1(area, is_vertical)](/cells/tr/python-net/aspose.cells.charts/seriescollection/add_r1c1/#str-bool) | [SeriesCollection](/cells/tr/python-net/aspose.cells.charts/seriescollection) koleksiyonunu bir grafiğe ekler.|
| [binary_search(item)](/cells/tr/python-net/aspose.cells.charts/seriescollection/binary_search/#Series) | Varsayılan karşılaştırıcıyı kullanarak sıralanmış dizi listesinin tamamında bir öğe arar ve öğenin sıfır tabanlı dizinini döndürür.|



###  Örnek

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "A4" cell
worksheet.cells.get("A4").put_value(200)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a sample value to "B4" cell
worksheet.cells.get("B4").put_value(40)
# Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").put_value("Q1")
# Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").put_value("Q2")
# Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").put_value("Y1")
# Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").put_value("Y2")
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# Saving the Excel file
workbook.save("book1.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells.charts](..)
* sınıf [Series](/cells/tr/python-net/aspose.cells.charts/series)
* sınıf [SeriesCollection](/cells/tr/python-net/aspose.cells.charts/seriescollection)
