---
title: طريقة is_chart_data_changed
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 70
url: /ar/python-net/aspose.cells.charts/chart/is_chart_data_changed/
is_root: false
---
##  is_chart_data_changed() {#}
يكتشف ما إذا كان قد تم تغيير مصدر بيانات المخطط.


###  عائدات

يعود صحيحًا إذا تم تغيير الرسم البياني وإلا فإنه يعود خطأ


```python
def is_chart_data_changed(self):
    ...
```


###  ملاحظات

تكتشف الطريقة التغييرات في مصدر بيانات المخطط قبل تحويل المخطط إلى تنسيق صورة.
في أول استدعاء Chart.toImage ، سيتم تسجيل بيانات مصدر المخطط (مثل XValuesParseData و ValuesParseData).
قبل استدعاء طريقة Chart.toImage مرة أخرى ، قم باستدعاء أسلوب IsChartDataChanged للتحقق مما إذا كان المخطط يحتاج إلى إعادة العرض.


###  أنظر أيضا
* وحدة [aspose.cells.charts](../../)
* فئة [Chart](/cells/ar/python-net/aspose.cells.charts/chart)
