---
title: "Series.CategoryValues"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تحصل على قيم الفئات الفعلية المستخدمة لرسم كل نقطة من هذه السلسلة في المخطط"
type: docs
url: /ar/net/aspose.cells.charts/series/categoryvalues/
---
## Series.CategoryValues property

يحصل على قيم الفئات الفعلية المستخدمة لرسم كل نقطة من هذه السلسلة في المخطط.

```csharp
public ChartDataValue[][] CategoryValues { get; }
```

### ملاحظات

توفر هذه الخاصية طريقة مريحة للحصول على القيم الفعلية المقابلة للبيانات المعرفة بواسطة [`XValues`](../xvalues/)، خاصة عندما يكون مصدر البيانات المحدد رابطًا خارجيًا أو صيغةً، ...إلخ.

### أمثلة

```csharp
//عرض توضيحي لإظهار حالة واحدة تتطلب هذه الخاصية:
[C#]

//مثال مستقل
Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string XValues = chart.NSeries[0].XValues;
// قد تكون XValues مثل \"[External.xlsx]Sheet1!$B$2:$C$6\" وهو أمر معقد
// للمستخدم للحصول على القيم الفعلية (قد تكون القيم مرتبطة بدفتر عمل آخر،
// أو مخزنة مؤقتًا في المصنف الحالي). هنا يمكنك استخدام خاصية CategoryValues
// للحصول على قيم الفئات المعروضة فعليًا في واجهة Excel
// على شكل مصفوفة ثنائية الأبعاد.
ChartDataValue[][] v1 = chart.NSeries[0].CategoryValues;

```

### انظر أيضًا

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


