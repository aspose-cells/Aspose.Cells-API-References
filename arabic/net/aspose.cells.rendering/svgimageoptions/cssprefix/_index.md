---
title: "SvgImageOptions.CssPrefix"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SvgImageOptions. تحصل وتعيّن بادئة اسم الـ CSS في SVG. القيمة الافتراضية هي سلسلة فارغة"
type: docs
url: /ar/net/aspose.cells.rendering/svgimageoptions/cssprefix/
---
## SvgImageOptions.CssPrefix property

يحصل ويضبط بادئة اسم CSS في SVG، القيمة الافتراضية هي سلسلة فارغة.

```csharp
public string CssPrefix { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyCssPrefixDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue(2019);
            worksheet.Cells["A3"].PutValue(2020);
            worksheet.Cells["A4"].PutValue(2021);
            worksheet.Cells["A5"].PutValue(2022);

            worksheet.Cells["B2"].PutValue(4500);
            worksheet.Cells["B3"].PutValue(4900);
            worksheet.Cells["B4"].PutValue(5200);
            worksheet.Cells["B5"].PutValue(6100);

            // إنشاء مخطط خطي
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B5", true);

            // إنشاء خيارات صورة SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // عرض بادئة CSS الحالية
            Console.WriteLine("Current CssPrefix value: " + svgOptions.CssPrefix);

            // تعيين بادئة CSS جديدة
            svgOptions.CssPrefix = "chart-prefix-";

            // عرض توليد SVG مع بادئة CSS مخصصة
            string outputPath = "output_chart.svg";
            chart.ToImage(outputPath, svgOptions);

            Console.WriteLine("Chart saved as SVG with custom CSS prefix.");
        }
    }
}
```

### انظر أيضًا

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


