---
title: "GridPivotTable.CalculateData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridPivotTable. تحسب بيانات الجداول المحورية إلى الخلايا"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridpivottable/calculatedata/
---
## GridPivotTable.CalculateData method

يحسب بيانات pivottable إلى الخلايا.

```csharp
public void CalculateData()
```

### ملاحظات

Cell.Value في نطاق المحور لا يمكنه إرجاع النتيجة الصحيحة إذا لم يتم استدعاء الطريقة. هذه الطريقة تحسب البيانات باستخدام ذاكرة تخزين مؤقت داخلية للمحور، وليس مصدر البيانات الأصلي. لذا إذا تم تغيير مصدر البيانات، يرجى استدعاء طريقة RefreshData() أولاً.

### انظر أيضًا

* class [GridPivotTable](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


