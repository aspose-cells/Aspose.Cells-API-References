---
title: "SvgImageOptions.CssPrefix"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SvgImageOptions özelliği. SVG'deki css adının önekini alır ve ayarlar; varsayılan değer boş dizedir."
type: docs
url: /tr/net/aspose.cells.rendering/svgimageoptions/cssprefix/
---
## SvgImageOptions.CssPrefix property

Svg içinde css adının önekini alır ve ayarlar, varsayılan değer boş dizedir.

```csharp
public string CssPrefix { get; set; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
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

            // Bir çizgi grafik oluştur
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B5", true);

            // SVG görüntü seçenekleri oluştur
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Mevcut CSS önekini göster
            Console.WriteLine("Current CssPrefix value: " + svgOptions.CssPrefix);

            // Yeni CSS önekini ayarla
            svgOptions.CssPrefix = "chart-prefix-";

            // Özel CSS önekiyle SVG oluşturmayı göster
            string outputPath = "output_chart.svg";
            chart.ToImage(outputPath, svgOptions);

            Console.WriteLine("Chart saved as SVG with custom CSS prefix.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


