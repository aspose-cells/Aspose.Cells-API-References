---
title: "SeriesLayoutProperties.ShowMeanLine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SeriesLayoutProperties. تشير إلى ما إذا كان سيتم إظهار الخط الذي يربط جميع نقاط المتوسط"
type: docs
url: /ar/net/aspose.cells.charts/serieslayoutproperties/showmeanline/
---
## SeriesLayoutProperties.ShowMeanLine property

يشير إلى ما إذا كان يجب إظهار الخط الذي يربط جميع نقاط المتوسط.

```csharp
public bool ShowMeanLine { get; set; }
```

### ملاحظات

يعمل فقط مع مخطط BoxWhisker.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanLineDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لمخطط الصندوق والشارب
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(25);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(115);
            worksheet.Cells["A7"].PutValue(65.666);

            // أضف مخطط الصندوق والشارب
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة إلى المخطط
            chart.NSeries.Add("A1:A7", true);

            // احصل على السلسلة الأولى
            Series series = chart.NSeries[0];

            // الوصول إلى خصائص التخطيط
            SeriesLayoutProperties layout = series.LayoutProperties;

            // عرض خاصية ShowMeanLine
            Console.WriteLine("Default ShowMeanLine value: " + layout.ShowMeanLine);
            
            // عيّن ShowMeanLine إلى true
            layout.ShowMeanLine = true;
            Console.WriteLine("After setting ShowMeanLine to true: " + layout.ShowMeanLine);

            // احفظ المصنف
            workbook.Save("BoxWhiskerChart_ShowMeanLineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


