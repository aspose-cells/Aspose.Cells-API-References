---
title: ScrollBarActiveXControl sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 100
url: /tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/
is_root: false
---
##  ScrollBarActiveXControl sınıfı
ScrollBar denetimini temsil eder.



**Miras:** [ScrollBarActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol) → 
[SpinButtonActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol) → 
[ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol) → 
[ActiveXControlBase](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)



ScrollBarActiveXControl türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [workbook](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/workbook) | [ActiveXControlBase.workbook](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase#workbook) nesnesini alır.|
| [type](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type) | ActiveX denetiminin türünü alır.|
| [width](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/width) |Denetimin genişliğini nokta birimleri cinsinden alır ve ayarlar.|
| [height](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/height) | Denetimin yüksekliğini nokta birimleri cinsinden alır ve ayarlar.|
| [mouse_icon](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_icon) | Denetim için fare işaretçisi olarak görüntülenecek özel bir simge alır ve ayarlar.|
| [mouse_pointer](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/mouse_pointer) | Denetim için fare işaretçisi olarak görüntülenen simge türünü alır ve ayarlar.|
| [fore_ole_color](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/fore_ole_color) | Ön planın ole rengini alır ve ayarlar.|
| [back_ole_color](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/back_ole_color) | Arka planın ole rengini alır ve ayarlar.|
| [is_visible](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_visible) | Bu kontrolün görünür olup olmadığını gösterir.|
| [shadow](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/shadow) | Gölge gösterilip gösterilmeyeceğini belirtir.|
| [linked_cell](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/linked_cell) | Bağlı hücreyi alır ve ayarlar.|
| [list_fill_range](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/list_fill_range) | Liste doldurma aralığını alır ve ayarlar.|
| [data](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/data) | Denetimin ikili verilerini alır ve ayarlar.|
| [is_enabled](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_enabled) | Denetimin odağı alıp alamayacağını ve kullanıcı tarafından oluşturulan olaylara yanıt verip veremeyeceğini belirtir.|
| [is_locked](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_locked) | Denetimdeki verilerin düzenleme için kilitli olup olmadığını gösterir.|
| [is_transparent](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_transparent) | Kontrolün şeffaf olup olmadığını gösterir.|
| [is_auto_size](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/is_auto_size) | Denetimin tüm içeriğini görüntülemek için otomatik olarak yeniden boyutlandırılıp boyutlandırılmayacağını belirtir.|
| [ime_mode](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/ime_mode) |Odağı alırken denetim için Giriş Yöntemi Düzenleyicisi'nin varsayılan çalışma zamanı modunu alır ve ayarlar.|
| [font](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/font) | Denetimin yazı tipini temsil eder.|
| [text_align](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/text_align) | Denetim tarafından kullanılan metnin nasıl hizalanacağını temsil eder.|
| [min](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/min) | Kabul edilebilir minimum değeri alır ve ayarlar.|
| [max](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/max) | Kabul edilebilir maksimum değeri alır ve ayarlar.|
| [position](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/position) | Değeri alır ve ayarlar.|
| [small_change](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/small_change) | Konum özelliğinin değiştiği miktarı alır ve ayarlar|
| [orientation](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/orientation) | SpinButton veya ScrollBar öğesinin dikey mi yoksa yatay mı yönlendirildiğini alır ve ayarlar.|
| [large_change](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/large_change) | Konum özelliğinin değiştiği miktarı alır ve ayarlar|



###  örnekler

```python
from aspose import pycore
from aspose.cells import Workbook
from aspose.cells.drawing.activexcontrols import ControlType, ScrollBarActiveXControl

# Initialize a new workbook.
book = Workbook()
# Add a ToggleButtonActiveXControl.
shape = book.worksheets[0].shapes.add_active_x_control(ControlType.SCROLL_BAR, 1, 0, 1, 0, 100, 50)
activeXControl = pycore.cast(ScrollBarActiveXControl, shape.active_x_control)
# do your business
# Save the excel file.
book.save("exmaple.xlsx")

```

###  Ayrıca bakınız
* modül [aspose.cells.drawing.activexcontrols](..)
* sınıf [ActiveXControl](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* sınıf [ActiveXControlBase](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/activexcontrolbase)
* sınıf [ScrollBarActiveXControl](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol)
* sınıf [SpinButtonActiveXControl](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol)
