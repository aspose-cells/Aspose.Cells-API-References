---
title: "Series.Move"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Series. تحرك السلسلة للأعلى أو للأسفل"
type: docs
url: /ar/net/aspose.cells.charts/series/move/
---
## Series.Move method

ينقل السلسلة للأعلى أو للأسفل.

```csharp
public void Move(int count)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عدد | Int32 | عدد الحركات صعودًا أو هبوطًا. حرك السلسلة للأعلى إذا كان هذا أقل من الصفر؛ حرك السلسلة للأسفل إذا كان هذا أكبر من الصفر. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesMethodMoveWithInt32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة إلى المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // احصل على السلسلة الأولى
            Series series = chart.NSeries[0];
            
            try
            {
                // استدعِ طريقة Move مع معامل Int32
                series.Move(1);
                
                Console.WriteLine("Series moved successfully by 1 position");
                
                // اعرض التأثير بتغيير اسم السلسلة
                series.Name = "Moved Series";
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("SeriesMethodMoveWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


