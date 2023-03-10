---
title: WorkbookDesigner sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1600
url: /tr/python-net/aspose.cells/workbookdesigner/
is_root: false
---
##  WorkbookDesigner sınıfı
Bir tasarımcı elektronik tablosunu temsil eden nesneyi kapsüller.



WorkbookDesigner türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [WorkbookDesigner()](/cells/tr/python-net/aspose.cells/workbookdesigner/__init__/#) | [WorkbookDesigner](/cells/tr/python-net/aspose.cells/workbookdesigner) sınıfının yeni bir örneğini başlatır.|
| [WorkbookDesigner(workbook)](/cells/tr/python-net/aspose.cells/workbookdesigner/__init__/#Workbook) | [WorkbookDesigner](/cells/tr/python-net/aspose.cells/workbookdesigner) sınıfının yeni bir örneğini başlatır.|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [workbook](/cells/tr/python-net/aspose.cells/workbookdesigner/workbook) |[WorkbookDesigner.workbook](/cells/tr/python-net/aspose.cells/workbookdesigner#workbook) nesnesini alır ve ayarlar.|
| [repeat_formulas_with_subtotal](/cells/tr/python-net/aspose.cells/workbookdesigner/repeat_formulas_with_subtotal) | Ara toplam satırı ile formüllerin tekrarlanıp tekrarlanmadığını gösterir.|
| [update_empty_string_as_null](/cells/tr/python-net/aspose.cells/workbookdesigner/update_empty_string_as_null) | DOĞRU ise, değer "" ise Null eklenecektir;|
| [update_reference](/cells/tr/python-net/aspose.cells/workbookdesigner/update_reference) |Diğer çalışma sayfalarındaki başvuruların güncellenip güncellenmeyeceğini belirtir.|
| [calculate_formula](/cells/tr/python-net/aspose.cells/workbookdesigner/calculate_formula) | Formüllerin hesaplanıp hesaplanmayacağını belirtir.|
| [call_back](/cells/tr/python-net/aspose.cells/workbookdesigner/call_back) | Smartmarker işlemenin geri arama arayüzünü alır ve ayarlar.|
| [line_by_line](/cells/tr/python-net/aspose.cells/workbookdesigner/line_by_line) | Akıllı işaretleyicinin satır satır işlenip işlenmediğini gösterir.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_data_source(data_source, cells_data_table)](/cells/tr/python-net/aspose.cells/workbookdesigner/set_data_source/#str-ICellsDataTable) | [ICellsDataTable](/cells/tr/python-net/aspose.cells/icellsdatatable) nesnesinin veri kaynağını ayarlar.|
| [set_data_source(variable, data)](/cells/tr/python-net/aspose.cells/workbookdesigner/set_data_source/#str-any) | Veri bağlamayı bir değişkene ayarlar.|
| [process()](/cells/tr/python-net/aspose.cells/workbookdesigner/process/#) | Akıllı işaretleyicileri işler ve veri kaynağı değerlerini doldurur.|
| [process(is_preserved)](/cells/tr/python-net/aspose.cells/workbookdesigner/process/#bool) | Akıllı işaretleyicileri işler ve veri kaynağı değerlerini doldurur.|
| [process(sheet_index, is_preserved)](/cells/tr/python-net/aspose.cells/workbookdesigner/process/#int-bool) | Akıllı işaretleyicileri işler ve veri kaynağı değerlerini doldurur.|
| [clear_data_source()](/cells/tr/python-net/aspose.cells/workbookdesigner/clear_data_source/#) | Tüm veri kaynaklarını temizler.|
| [get_smart_markers()](/cells/tr/python-net/aspose.cells/workbookdesigner/get_smart_markers/#) | Bir elektronik tablodaki akıllı işaretçilerin bir koleksiyonunu döndürür.|



###  Örnek

```python
from aspose.cells import Workbook, WorkbookDesigner

# Create WorkbookDesigner object.
wd = WorkbookDesigner()
# Open the template file (which contains smart markers).
wd.workbook = Workbook("SmartMarker_Designer.xls")
# Initialize your data from data source
# DataSet ds = new DataSet();
# ...
# Set the datatable as the data source.
# wd.SetDataSource(dt);
# Process the smart markers to fill the data into the worksheets.
wd.process(True)
# Save the excel file.
wd.workbook.save("outSmartMarker_Designer.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [ICellsDataTable](/cells/tr/python-net/aspose.cells/icellsdatatable)
* sınıf [WorkbookDesigner](/cells/tr/python-net/aspose.cells/workbookdesigner)
