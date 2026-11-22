---
title: "Chart.SizeWithWindow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المخطط. صحيحة إذا كان Microsoft Excel يعيد تحجيم المخطط ليتطابق مع حجم نافذة ورقة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/chart/sizewithwindow/
---
## Chart.SizeWithWindow property

صحيح إذا كان Microsoft Excel يعيد تحجيم المخطط ليتطابق مع حجم نافذة ورقة المخطط.

```csharp
public bool SizeWithWindow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySizeWithWindowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // عرض خاصية SizeWithWindow
            Console.WriteLine("Default SizeWithWindow: " + chart.SizeWithWindow);
            
            // تمكين SizeWithWindow
            chart.SizeWithWindow = true;
            Console.WriteLine("After setting SizeWithWindow to true: " + chart.SizeWithWindow);
            
            // احفظ المصنف
            workbook.Save("ChartSizeWithWindowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


