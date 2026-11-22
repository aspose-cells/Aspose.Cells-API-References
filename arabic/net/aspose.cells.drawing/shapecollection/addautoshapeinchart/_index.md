---
title: "ShapeCollection.AddAutoShapeInChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تُضيف AutoShape إلى المخطط"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addautoshapeinchart/
---
## ShapeCollection.AddAutoShapeInChart method

يضيف AutoShape إلى المخطط.

```csharp
public Shape AddAutoShapeInChart(AutoShapeType type, int top, int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | AutoShapeType | نوع الشكل التلقائي. |
| أعلى | Int32 | يمثل الإزاحة العمودية لمربع النص من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| يسار | Int32 | يمثل الإزاحة العمودية لمربع النص من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| الارتفاع | Int32 | يمثل ارتفاع مربع النص بوحدات 1/4000 من مساحة المخطط. |
| العرض | Int32 | يمثل عرض مربع النص بوحدات 1/4000 من مساحة المخطط. |

### قيمة الإرجاع

يعيد كائن شكل.

### ملاحظات

النوع لا يمكن أن يكون Chart/Comment/Picture/OleObject/Polygon/DialogBox

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddAutoShapeInChartWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // استدعِ طريقة AddAutoShapeInChart لإضافة شكل نجمة إلى المخطط.
                Shape shape = chart.Shapes.AddAutoShapeInChart(
                    AutoShapeType.Star16,  // AutoShapeType
                    100,                  // Top position (in pixels)
                    100,                  // Left position (in pixels)
                    200,                  // Height (in pixels)
                    200);                 // Width (in pixels)

                // تعيين خصائص الشكل
                shape.Name = "SampleStar";
                shape.Fill.SolidFill.Color = System.Drawing.Color.Yellow;
                shape.Line.SolidFill.Color = System.Drawing.Color.Red;

                Console.WriteLine("Star shape added successfully to the chart.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAutoShapeInChart method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("ShapeCollectionMethodAddAutoShapeInChartDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


