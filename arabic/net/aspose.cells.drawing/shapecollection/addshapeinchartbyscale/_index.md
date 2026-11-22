---
title: "ShapeCollection.AddShapeInChartByScale"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. إضافة شكل إلى المخطط. جميع الوحدات هي النسبة المئوية لمساحة المخطط"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addshapeinchartbyscale/
---
## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double) {#addshapeinchartbyscale}

أضف شكلاً إلى المخطط. كل وحدة هي النسبة المئوية من مساحة المخطط.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | MsoDrawingType | نوع الرسم. |
| الموضع | PlacementType | نوع الموضع. |
| يسار | Double | الوحدة هي النسبة المئوية لعرض مساحة المخطط. |
| أعلى | Double | الوحدة هي النسبة المئوية لارتفاع مساحة المخطط. |
| يمين | Double | الوحدة هي النسبة المئوية لعرض مساحة المخطط. |
| أسفل | Double | الوحدة هي النسبة المئوية لارتفاع مساحة المخطط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeInChartByScaleWithMsoDrawingTypePlacementTypeDouDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // حساب المخطط
            chart.Calculate();

            // إضافة شكل مستطيل إلى المخطط باستخدام إحداثيات النسبة المئوية
            Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle, 
                PlacementType.Move,
                0.2,  // x1 (20% from left)
                0.2,  // y1 (20% from top)
                0.4,  // x2 (40% from left)
                0.4); // y2 (40% from top)
            rectangle.Fill.SolidFill.Color = Color.Blue;
            rectangle.Line.SolidFill.Color = Color.Black;

            // إضافة شكل بيضاوي إلى المخطط باستخدام إحداثيات النسبة المئوية
            Shape oval = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Oval,
                PlacementType.Move,
                0.6,  // x1 (60% from left)
                0.6,  // y1 (60% from top)
                0.8,  // x2 (80% from left)
                0.8); // y2 (80% from top)
            oval.Fill.SolidFill.Color = Color.Red;
            oval.Line.SolidFill.Color = Color.Black;

            // احفظ المصنف
            workbook.Save("AddShapeInChartByScaleWithMsoDrawingType.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double, byte[]) {#addshapeinchartbyscale_1}

أضف شكلاً إلى المخطط. كل وحدة هي 1/4000 من مساحة المخطط.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom, byte[] imageData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | MsoDrawingType | نوع الرسم. |
| الموضع | PlacementType | نوع الموضع. |
| يسار | Double | الوحدة هي النسبة المئوية لعرض مساحة المخطط. |
| أعلى | Double | الوحدة هي النسبة المئوية لارتفاع مساحة المخطط. |
| يمين | Double | الوحدة هي النسبة المئوية لعرض مساحة المخطط. |
| أسفل | Double | الوحدة هي النسبة المئوية لارتفاع مساحة المخطط. |
| imageData | Byte[] | إذا لم يكن الشكل صورة أو كائن ole، يجب أن تكون imageData فارغة. |

### انظر أيضًا

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


