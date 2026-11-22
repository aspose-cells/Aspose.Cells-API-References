---
title: "ShapeCollection.AddLabelInChart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. تضيف تسمية إلى المخطط"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addlabelinchart/
---
## ShapeCollection.AddLabelInChart method

يضيف label إلى المخطط.

```csharp
public Label AddLabelInChart(int top, int left, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| أعلى | Int32 | يمثل الإزاحة العمودية للتسمية من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| يسار | Int32 | يمثل الإزاحة العمودية للتسمية من الزاوية العلوية اليسرى بوحدات 1/4000 من مساحة المخطط. |
| الارتفاع | Int32 | يمثل ارتفاع التسمية، بوحدات 1/4000 من مساحة المخطط. |
| العرض | Int32 | يمثل عرض التسمية، بوحدات 1/4000 من مساحة المخطط. |

### قيمة الإرجاع

كائن Label جديد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لإنشاء مخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];            
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // استدعِ طريقة AddLabelInChart مع المعلمات (top, left, height, width)
                Label label = chart.Shapes.AddLabelInChart(100, 100, 200, 200);
                
                // عيّن خصائص التسمية
                label.Text = "Sample Chart Label";
                label.Font.Color = System.Drawing.Color.Red;
                label.Font.Size = 12;

                Console.WriteLine("Label added successfully to chart with parameters (100, 100, 200, 50)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddLabelInChart method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


