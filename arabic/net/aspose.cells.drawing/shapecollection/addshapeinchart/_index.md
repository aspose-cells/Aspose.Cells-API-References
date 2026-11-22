---
title: "ShapeCollection.AddShapeInChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. إضافة شكل إلى المخطط. كل وحدة هي 1/4000 من مساحة المخطط"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addshapeinchart/
---
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int, byte[]) {#addshapeinchart_1}

أضف شكلاً إلى المخطط. كل وحدة هي 1/4000 من مساحة المخطط.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom, byte[] imageData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | MsoDrawingType | نوع الرسم. |
| الموضع | PlacementType | نوع الموضع. |
| يسار | Int32 | بوحدة 1/4000 من عرض مساحة المخطط. |
| أعلى | Int32 | بوحدة 1/4000 من ارتفاع مساحة المخطط. |
| يمين | Int32 | بوحدة 1/4000 من عرض مساحة المخطط. |
| أسفل | Int32 | بوحدة 1/4000 من ارتفاع مساحة المخطط. |
| imageData | Byte[] | إذا لم يكن الشكل صورة أو كائن ole، يجب أن تكون imageData فارغة. |

### انظر أيضًا

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int) {#addshapeinchart}

أضف شكلاً إلى المخطط. كل وحدة هي 1/4000 من مساحة المخطط.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | MsoDrawingType | نوع الرسم. |
| الموضع | PlacementType | نوع الموضع. |
| يسار | Int32 | بوحدة 1/4000 من عرض مساحة المخطط. |
| أعلى | Int32 | بوحدة 1/4000 من ارتفاع مساحة المخطط. |
| يمين | Int32 | بوحدة 1/4000 من عرض مساحة المخطط. |
| أسفل | Int32 | بوحدة 1/4000 من ارتفاع مساحة المخطط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddShapeInChartWithMsoDrawingTypePlacementTypeIntDemo
    {
        public static void Run()
        {
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // إضافة شكل إلى المخطط
            chart.Shapes.AddShapeInChart(MsoDrawingType.CheckBox, PlacementType.Move, 100, 100, 1000, 1000);
            
            // تعيين نص الشكل
            chart.Shapes[0].Text = "Sample CheckBox";
            
            // احفظ دفتر العمل
            workbook.Save("AddShapeInChartWithMsoDrawingType.xlsx");
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


