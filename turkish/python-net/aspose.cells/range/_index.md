---
title: Range sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1250
url: /tr/python-net/aspose.cells/range/
is_root: false
---
##  Range sınıfı
Bir elektronik tablodaki bir hücre aralığını temsil eden nesneyi kapsüller.



Range türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [current_region](/cells/tr/python-net/aspose.cells/range/current_region) |Geçerli bölgeyi temsil eden bir Range nesnesi döndürür.<br/> Geçerli bölge, boş satırların ve boş sütunların herhangi bir kombinasyonuyla sınırlanan bir aralıktır.|
| [hyperlinks](/cells/tr/python-net/aspose.cells/range/hyperlinks) | Aralıktaki tüm köprüleri alır.|
| [row_count](/cells/tr/python-net/aspose.cells/range/row_count) | Aralıktaki satır sayısını alır.|
| [column_count](/cells/tr/python-net/aspose.cells/range/column_count) | Aralıktaki sütun sayısını alır.|
| [cell_count](/cells/tr/python-net/aspose.cells/range/cell_count) | Aralıktaki tüm hücre sayısını alır.|
| [name](/cells/tr/python-net/aspose.cells/range/name) | Aralığın adını alır veya ayarlar.|
| [refers_to](/cells/tr/python-net/aspose.cells/range/refers_to) | Aralığın referanslarını alır.|
| [address](/cells/tr/python-net/aspose.cells/range/address) | Aralığın adresini alır.|
| [left](/cells/tr/python-net/aspose.cells/range/left) | A sütununun sol kenarından aralığın sol kenarına olan mesafeyi puan olarak alır.|
| [top](/cells/tr/python-net/aspose.cells/range/top) | 1. satırın üst kenarından aralığın üst kenarına olan mesafeyi puan olarak alır.|
| [width](/cells/tr/python-net/aspose.cells/range/width) | Puan aralığının genişliğini alır.|
| [height](/cells/tr/python-net/aspose.cells/range/height) | Puan aralığının genişliğini alır.|
| [first_row](/cells/tr/python-net/aspose.cells/range/first_row) | Aralığın ilk satırının indeksini alır.|
| [first_column](/cells/tr/python-net/aspose.cells/range/first_column) | Aralığın ilk sütununun dizinini alır.|
| [value](/cells/tr/python-net/aspose.cells/range/value) | Aralığın değerini alır ve ayarlar.|
| [column_width](/cells/tr/python-net/aspose.cells/range/column_width) | Bu aralığın sütun genişliğini ayarlar veya alır|
| [row_height](/cells/tr/python-net/aspose.cells/range/row_height) | Bu aralıktaki satırların yüksekliğini ayarlar veya alır|
| [entire_column](/cells/tr/python-net/aspose.cells/range/entire_column) |Belirtilen aralığı içeren tüm sütunu (veya sütunları) temsil eden bir Range nesnesi alır.|
| [entire_row](/cells/tr/python-net/aspose.cells/range/entire_row) | Belirtilen aralığı içeren tüm satırı (veya satırları) temsil eden bir Range nesnesi alır.|
| [worksheet](/cells/tr/python-net/aspose.cells/range/worksheet) | Bu aralığı içeren [Range.worksheet](/cells/tr/python-net/aspose.cells/range#worksheet) nesnesini alır.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [auto_fill(target)](/cells/tr/python-net/aspose.cells/range/auto_fill/#Range) | Hedef aralığı otomatik olarak doldurun.|
| [auto_fill(target, auto_fill_type)](/cells/tr/python-net/aspose.cells/range/auto_fill/#Range-AutoFillType) | Hedef aralığı otomatik olarak doldurun.|
| [set_style(style, explicit_flag)](/cells/tr/python-net/aspose.cells/range/set_style/#Style-bool) | Hücre stilini uygulayın.|
| [set_style(style)](/cells/tr/python-net/aspose.cells/range/set_style/#Style) | Aralığın stilini ayarlar.|
| [set_outline_borders(border_style, border_color)](/cells/tr/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-CellsColor) | Ana hat kenarlıklarını, aynı kenarlık stili ve rengine sahip bir hücre aralığının çevresine ayarlar.|
| [set_outline_borders(border_style, border_color)](/cells/tr/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-aspose.pydrawing.Color) | Ana hat kenarlıklarını, aynı kenarlık stili ve rengine sahip bir hücre aralığının çevresine ayarlar.|
| [set_outline_borders(border_styles, border_colors)](/cells/tr/python-net/aspose.cells/range/set_outline_borders/#list-aspose.pydrawing.Color[]) | Bir hücre aralığının etrafındaki çizgi kenarlıklarını ayarlar.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/tr/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-CellsColor) | Bir hücre aralığının çevresine anahat kenarlığı ayarlar.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/tr/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | Bir hücre aralığının çevresine anahat kenarlığı ayarlar.|
| [copy(range, options)](/cells/tr/python-net/aspose.cells/range/copy/#Range-PasteOptions) | Özel seçenekleri yapıştırarak aralığı kopyalama.|
| [copy(range)](/cells/tr/python-net/aspose.cells/range/copy/#Range) | Bir kaynak aralıktan verileri (formüller dahil), biçimlendirmeyi, çizim nesnelerini vb. kopyalar.|
| [get_enumerator()](/cells/tr/python-net/aspose.cells/range/get_enumerator/#) | Bu Aralıktaki hücreler için Numaralandırıcıyı alır.|
| [is_intersect(range)](/cells/tr/python-net/aspose.cells/range/is_intersect/#Range) | Aralığın kesişip kesişmediğini gösterir.|
| [intersect(range)](/cells/tr/python-net/aspose.cells/range/intersect/#Range) | İki aralığın dikdörtgen kesişimini temsil eden bir [Range](/cells/tr/python-net/aspose.cells/range) nesnesi döndürür.|
| [union(range)](/cells/tr/python-net/aspose.cells/range/union/#Range) | İki aralığın birleşimini döndürür.|
| [merge()](/cells/tr/python-net/aspose.cells/range/merge/#) | Bir dizi hücreyi tek bir hücrede birleştirir.|
| [un_merge()](/cells/tr/python-net/aspose.cells/range/un_merge/#) |Bu aralığın birleştirilmiş hücrelerini ayırır.|
| [put_value(string_value, is_converted, set_style)](/cells/tr/python-net/aspose.cells/range/put_value/#str-bool-bool) | Aralığa bir değer koyar, uygunsa değer diğer veri tipine dönüştürülür ve hücrenin sayı formatı sıfırlanır.|
| [apply_style(style, flag)](/cells/tr/python-net/aspose.cells/range/apply_style/#Style-StyleFlag) | Biçimleri tüm aralık için uygular.|
| [set_inside_borders(border_edge, line_style, border_color)](/cells/tr/python-net/aspose.cells/range/set_inside_borders/#BorderType-CellBorderType-CellsColor) | Aralığın sınırları içinde ayarlayın.|
| [move_to(dest_row, dest_column)](/cells/tr/python-net/aspose.cells/range/move_to/#int-int) | Geçerli aralığı hedef aralığa taşıyın.|
| [copy_data(range)](/cells/tr/python-net/aspose.cells/range/copy_data/#Range) | Bir kaynak aralığından hücre verilerini (formüller dahil) kopyalar.|
| [copy_value(range)](/cells/tr/python-net/aspose.cells/range/copy_value/#Range) | Hücre değerini bir kaynak aralıktan kopyalar.|
| [copy_style(range)](/cells/tr/python-net/aspose.cells/range/copy_style/#Range) | Bir kaynak aralığından stil ayarlarını kopyalar.|
| [get_cell_or_null(row_offset, column_offset)](/cells/tr/python-net/aspose.cells/range/get_cell_or_null/#int-int) | Bu aralıkta [Cell](/cells/tr/python-net/aspose.cells/cell) nesnesi veya boş değer alır.|
| [get_offset(row_offset, column_offset)](/cells/tr/python-net/aspose.cells/range/get_offset/#int-int) | Ofset ile [Range](/cells/tr/python-net/aspose.cells/range) aralığını alır.|



###  Örnek

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
#  Create a range (A1:D3).
range = cells.create_range("A1", "D3")
#  Set value to the range.
range.value = "Hello"
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [Cell](/cells/tr/python-net/aspose.cells/cell)
* sınıf [Range](/cells/tr/python-net/aspose.cells/range)
