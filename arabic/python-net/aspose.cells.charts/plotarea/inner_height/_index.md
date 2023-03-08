---
title: inner_height الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 150
url: /ar/python-net/aspose.cells.charts/plotarea/inner_height/
is_root: false
---
##  inner_height الملكية

الحصول على ارتفاع مساحة الرسم أو تعيينه بوحدات 1/4000 من مساحة المخطط.

###  ملاحظات

يشتمل المربع المحيط بمنطقة الرسم على منطقة الرسم وعلامات التجزئة (تسميات التجزئة) وحدًا صغيرًا حول علامات التجزئة.
إذا لم يتم إنشاء القيمة بواسطة MS Excel ، يرجى الاتصال بطريقة Chart.Calculate () قبل استدعاء هذه الطريقة.


 ال**X ** ، ** ص** , **عرض** و**ارتفاع** ل**قطعة أرض** يمثل مساحة قطعة الأرض
 المربع المحيط الذي يتضمن منطقة الرسم ، وعلامات التجزئة (تسميات التجزئة) ، وحد صغير حول علامات التجزئة.
 إذا كنت ترغب في الحصول على الحجم الفعلي لمنطقة قطعة الأرض ، يجب عليك الاتصال**InnerX** , **الداخلية** , **العرض الداخلي** و
**الارتفاع الداخلي** ملكيات.


بالنسبة لبرنامج Excel 2007 أو الأخير ، تكون القيمة الافتراضية هي صفر. يجب عليك استدعاء الحصول على القيمة بعد استدعاء Chart.Calculate ().
###  تعريف:
```python
@property
def inner_height(self):
    ...
@inner_height.setter
def inner_height(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells.charts](../../)
* فئة [PlotArea](/cells/ar/python-net/aspose.cells.charts/plotarea)
