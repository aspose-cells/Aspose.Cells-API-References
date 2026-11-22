---
title: "Series.PointValues"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. يحصل على القيم الفعلية التي تُستخدم لرسم كل نقطة من هذه السلسلة في المخطط"
type: docs
url: /ar/net/aspose.cells.charts/series/pointvalues/
---
## Series.PointValues property

يحصل على القيم الفعلية المستخدمة لرسم كل نقطة من هذه السلسلة في المخطط.

```csharp
public ChartDataValue[] PointValues { get; }
```

### ملاحظات

توفر هذه الخاصية طريقة مريحة للحصول على القيم الفعلية المقابلة للبيانات المعرفة بواسطة [`Values`](../values/)، خاصة عندما يكون مصدر البيانات المحدد رابطًا خارجيًا أو صيغةً، ...إلخ.

### أمثلة

```csharp
//عرض توضيحي لإظهار حالة واحدة تتطلب هذه الخاصية:
[C#]

Workbook workbook = new Workbook("ExternalSourceChart.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
Chart chart = worksheet.Charts[0];
chart.Calculate();
string Values = chart.NSeries[0].Values;
// يمكن أن تكون القيم مثل "[External.xlsx]Sheet1!$A$1:$A$6" والتي تكون معقدة
// للمستخدم للحصول على القيم الفعلية (قد تكون القيم مرتبطة بدفتر عمل آخر،
// أو مخزنة مؤقتًا في دفتر العمل الحالي). هنا يمكنك استخدام خاصية PointValues
// للحصول على القيم المعروضة فعليًا في واجهة Excel
// في شكل مصفوفة.
ChartDataValue[] v1 = chart.NSeries[0].PointValues;

```

### انظر أيضًا

* class [ChartDataValue](../../chartdatavalue/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


