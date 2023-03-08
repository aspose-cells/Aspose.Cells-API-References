---
title: طريقة is_gather_string
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 20
url: /ar/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/
is_root: false
---
##  is_gather_string() {#}
للتحقق مما إذا كانت قيمة السلسلة الحالية للخلية بحاجة إلى أن يتم تجميعها في تجمع عمومي.


###  عائدات

صواب إذا كانت قيمة السلسلة بحاجة إلى أن يتم تجميعها في تجمع عام للملف الناتج.


```python
def is_gather_string(self):
    ...
```


###  ملاحظات

سيستفيد تجميع قيم السلسلة فقط عندما يكون هناك العديد من قيم السلسلة المكررة للخلايا التي يوفرها هذا التطبيق.
في هذه الحالة ، ستوفر سلسلة التجميع الكثير من الذاكرة وتولد ملفًا ناتجًا أصغر.
إذا كان هناك العديد من قيم السلسلة للخلايا التي يوفرها LightCellsDataProvider ولكن القليل منها متماثل ،
ستكلف سلسلة التجميع مزيدًا من الذاكرة والوقت وليس لها أي ميزة للملف الناتج.


###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [LightCellsDataProvider](/cells/ar/python-net/aspose.cells/lightcellsdataprovider)
