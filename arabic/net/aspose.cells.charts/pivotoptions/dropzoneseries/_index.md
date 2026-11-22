---
title: "PivotOptions.DropZoneSeries"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotOptions. تحدد ما إذا كان التحكم لكل حقل PivotTable على محور عمود PivotTable في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مضبوطة على true"
type: docs
url: /ar/net/aspose.cells.charts/pivotoptions/dropzoneseries/
---
## PivotOptions.DropZoneSeries property

يحدد ما إذا كان عنصر التحكم لكل حقل PivotTable على محور الأعمدة في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مُعينة إلى true.

```csharp
public bool DropZoneSeries { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneSeriesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل والحصول على الورقة الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(7);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("A1:B4", true);
            
            // الحصول على خيارات pivot من المخطط
            PivotOptions options = chart.PivotOptions;
            
            // عرض خاصية DropZoneSeries
            Console.WriteLine("Original DropZoneSeries value: " + options.DropZoneSeries);
            options.DropZoneSeries = true;
            Console.WriteLine("Modified DropZoneSeries value: " + options.DropZoneSeries);
            
            // احفظ المصنف
            workbook.Save("PivotOptionsPropertyDropZoneSeriesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


