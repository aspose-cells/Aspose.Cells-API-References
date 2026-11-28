---
title: "SvgImageOptions.SvgImageOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SvgImageOptions yapıcı. Ctor"
type: docs
url: /tr/net/aspose.cells.rendering/svgimageoptions/svgimageoptions/
---
## SvgImageOptions constructor

Yapıcı.

```csharp
public SvgImageOptions()
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Month");
            worksheet.Cells["A2"].PutValue("Jan");
            worksheet.Cells["A3"].PutValue("Feb");
            worksheet.Cells["A4"].PutValue("Mar");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(210);
            worksheet.Cells["B4"].PutValue(150);

            // Bir çizgi grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Yapıcıyı kullanarak SvgImageOptions oluştur
                SvgImageOptions svgOptions = new SvgImageOptions();

                // SVG renderleme seçeneklerini yapılandırın
                svgOptions.ImageType = ImageType.Svg; // Explicitly set to SVG
                svgOptions.FitToViewPort = true;
                svgOptions.CssPrefix = "chart-prefix";
                svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

                // Grafiği belirtilen seçeneklerle SVG olarak kaydet
                chart.ToImage("output_chart.svg", svgOptions);

                Console.WriteLine("SVG image saved successfully with specified options.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error generating SVG: {ex.Message}");
            }

            // Orijinal verileri göstermek için çalışma kitabını kaydet
            workbook.Save("SvgImageOptionsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


