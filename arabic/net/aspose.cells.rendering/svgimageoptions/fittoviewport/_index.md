---
title: "SvgImageOptions.FitToViewPort"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SvgImageOptions. إذا كانت هذه الخاصية true فإن الـ svg المولد سيتناسب مع مساحة العرض"
type: docs
url: /ar/net/aspose.cells.rendering/svgimageoptions/fittoviewport/
---
## SvgImageOptions.FitToViewPort property

إذا كانت هذه الخاصية true، فإن SVG المُولد سيتناسب مع منطقة العرض.

```csharp
public bool FitToViewPort { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsPropertyFitToViewPortDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // املأ الخلايا ببيانات تجريبية
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 250;

            // إنشاء مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 18, 6);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            chart.Title.Text = "Sales Report";

            // إنشاء خيارات عرض SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // عرض القيمة الأولية لـ FitToViewPort
            Console.WriteLine($"Initial FitToViewPort: {svgOptions.FitToViewPort}");

            // تعديل الخاصية وإظهار التأثير
            svgOptions.FitToViewPort = true;
            Console.WriteLine($"Modified FitToViewPort: {svgOptions.FitToViewPort}");

            // عرض ورقة العمل كـ SVG بإعدادات مختلفة
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortEnabled.svg");

            // اختياري: إنشاء مقارنة مع تعطيل FitToViewPort
            svgOptions.FitToViewPort = false;
            renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortDisabled.svg");

            Console.WriteLine("Generated SVG files demonstrate FitToViewPort effect.");
        }
    }
}
```

### انظر أيضًا

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


