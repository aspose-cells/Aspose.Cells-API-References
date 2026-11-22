---
title: "DataLabels.ApplyFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة DataLabels. تطبيق خط تسميات البيانات على جميع العقد الفرعية"
type: docs
url: /ar/net/aspose.cells.charts/datalabels/applyfont/
---
## DataLabels.ApplyFont method

تطبيق خط تسميات البيانات على جميع العقد الفرعية.

```csharp
public void ApplyFont()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsMethodApplyFontDemo
    {
        public static void Run()
        {
            // إنشاء مصنف والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // إظهار تسميات البيانات
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // تعيين لون خط جديد لتسميات البيانات
            Color newColor = Color.Green;
            series.DataLabels.Font.Color = newColor;
            
            // تطبيق إعدادات الخط على جميع تسميات البيانات
            series.DataLabels.ApplyFont();
            
            // احفظ المصنف
            workbook.Save("DataLabelsApplyFontDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


