---
title: Slicer sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 10
url: /tr/python-net/aspose.cells.slicers/slicer/
is_root: false
---
##  Slicer sınıfı
özet açıklama Slicer Görüntüle



Slicer türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [title](/cells/tr/python-net/aspose.cells.slicers/slicer/title) | Geçerli Dilimleyici nesnesinin başlığını belirtir.|
| [alternative_text](/cells/tr/python-net/aspose.cells.slicers/slicer/alternative_text) | Slicer nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar.|
| [is_printable](/cells/tr/python-net/aspose.cells.slicers/slicer/is_printable) | Dilimleyici nesnesinin yazdırılabilir olup olmadığını gösterir.|
| [is_locked](/cells/tr/python-net/aspose.cells.slicers/slicer/is_locked) | Dilimleyici şeklinin kilitli olup olmadığını gösterir.|
| [placement](/cells/tr/python-net/aspose.cells.slicers/slicer/placement) | Çizim nesnesinin altındaki hücrelere iliştirilme şeklini temsil eder.<br/> Özellik, bir nesnenin çalışma sayfasındaki yerleşimini kontrol eder.|
| [locked_aspect_ratio](/cells/tr/python-net/aspose.cells.slicers/slicer/locked_aspect_ratio) | En boy oranının kilitlenip kilitlenmediğini gösterir.|
| [locked_position](/cells/tr/python-net/aspose.cells.slicers/slicer/locked_position) | Belirtilen dilimleyicinin kullanıcı arabirimi kullanılarak taşınabileceğini veya yeniden boyutlandırılabileceğini gösterir.|
| [slicer_cache](/cells/tr/python-net/aspose.cells.slicers/slicer/slicer_cache) |Dilimleyiciyle ilişkili SlicerCache nesnesini döndürür.|
| [parent](/cells/tr/python-net/aspose.cells.slicers/slicer/parent) | Dilimleyiciyi içeren sayfayı temsil eden Worksheet nesnesini döndürür.|
| [style_type](/cells/tr/python-net/aspose.cells.slicers/slicer/style_type) | Yerleşik dilimleyici stilinin türünü belirtin<br/> varsayılan tür SlicerStyleLight1'dir.|
| [name](/cells/tr/python-net/aspose.cells.slicers/slicer/name) | Belirtilen dilimleyicinin adını döndürür veya ayarlar|
| [caption](/cells/tr/python-net/aspose.cells.slicers/slicer/caption) | Belirtilen dilimleyicinin başlığını döndürür veya ayarlar.|
| [caption_visible](/cells/tr/python-net/aspose.cells.slicers/slicer/caption_visible) | Dilimleyici Resim Yazısını görüntüleyen başlığın görünür olup olmadığını döndürür veya ayarlar<br/> varsayılan değer doğrudur|
| [number_of_columns](/cells/tr/python-net/aspose.cells.slicers/slicer/number_of_columns) | Belirtilen dilimleyicideki sütun sayısını döndürür veya ayarlar.|
| [left_pixel](/cells/tr/python-net/aspose.cells.slicers/slicer/left_pixel) | Dilimleyici şeklinin sol sütunundan yatay uzaklığını piksel cinsinden döndürür veya ayarlar.|
| [top_pixel](/cells/tr/python-net/aspose.cells.slicers/slicer/top_pixel) | Dilimleyici şeklinin üst satırından dikey uzaklığını piksel cinsinden döndürür veya ayarlar.|
| [width](/cells/tr/python-net/aspose.cells.slicers/slicer/width) | Belirtilen dilimleyicinin genişliğini nokta cinsinden döndürür veya ayarlar.|
| [width_pixel](/cells/tr/python-net/aspose.cells.slicers/slicer/width_pixel) | Belirtilen dilimleyicinin genişliğini piksel cinsinden döndürür veya ayarlar.|
| [height](/cells/tr/python-net/aspose.cells.slicers/slicer/height) | Belirtilen dilimleyicinin yüksekliğini nokta cinsinden döndürür veya ayarlar.|
| [height_pixel](/cells/tr/python-net/aspose.cells.slicers/slicer/height_pixel) |Belirtilen dilimleyicinin yüksekliğini piksel cinsinden döndürür veya ayarlar.|
| [column_width_pixel](/cells/tr/python-net/aspose.cells.slicers/slicer/column_width_pixel) | Dilimleyicinin her sütunu için genişliği piksel cinsinden alır veya ayarlar.|
| [column_width](/cells/tr/python-net/aspose.cells.slicers/slicer/column_width) | Dilimleyicideki her sütunun genişliğini punto cinsinden döndürür veya ayarlar.|
| [row_height_pixel](/cells/tr/python-net/aspose.cells.slicers/slicer/row_height_pixel) | Belirtilen dilimleyicideki her satırın yüksekliğini piksel cinsinden döndürür veya ayarlar.|
| [row_height](/cells/tr/python-net/aspose.cells.slicers/slicer/row_height) | Belirtilen dilimleyicideki her satırın punto cinsinden yüksekliğini döndürür veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [add_pivot_connection(pivot)](/cells/tr/python-net/aspose.cells.slicers/slicer/add_pivot_connection/#aspose.cells.pivot.PivotTable) | PivotTable bağlantısı ekler.|
| [remove_pivot_connection(pivot)](/cells/tr/python-net/aspose.cells.slicers/slicer/remove_pivot_connection/#aspose.cells.pivot.PivotTable) | PivotTable bağlantılarını kaldırır.|
| [refresh()](/cells/tr/python-net/aspose.cells.slicers/slicer/refresh/#) | Dilimleyici yenileniyor Bu arada, Göreli PivotTable'lar Yenileniyor ve Hesaplanıyor.|



###  örnekler

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
from aspose.cells.slicers import SlicerStyleType

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
pivot.refresh_data()
pivot.calculate_data()
slicers = sheet.slicers
slicerIndex = slicers.add(pivot, "E12", "fruit")
slicer = slicers[slicerIndex]
slicer.style_type = SlicerStyleType.SLICER_STYLE_LIGHT2
items = slicer.slicer_cache.slicer_cache_items
item = items[0]
item.selected = False
# do your business
book.save("out.xlsx")

```

###  Ayrıca bakınız
* modül [aspose.cells.slicers](..)
