---
title: "SvgImageOptions.FitToViewPort"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SvgImageOptions özelliği. Bu özellik true ise oluşturulan svg görünüm alanına sığacaktır"
type: docs
url: /tr/net/aspose.cells.rendering/svgimageoptions/fittoviewport/
---
## SvgImageOptions.FitToViewPort property

Bu özellik true ise, oluşturulan svg görüntüleme alanına sığar.

```csharp
public bool FitToViewPort { get; set; }
```

### Örnekler

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
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücreleri örnek veriyle doldurun
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 250;

            // Sütun grafik oluşturun
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 18, 6);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            chart.Title.Text = "Sales Report";

            // SVG renderleme seçenekleri oluştur
            SvgImageOptions svgOptions = new SvgImageOptions();

            // İlk FitToViewPort değerini göster
            Console.WriteLine($"Initial FitToViewPort: {svgOptions.FitToViewPort}");

            // Özelliği değiştir ve etkiyi göster
            svgOptions.FitToViewPort = true;
            Console.WriteLine($"Modified FitToViewPort: {svgOptions.FitToViewPort}");

            // Çalışma sayfasını farklı ayarlarla SVG'ye dönüştür
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortEnabled.svg");

            // İsteğe bağlı: FitToViewPort devre dışı bırakılmış bir karşılaştırma oluştur
            svgOptions.FitToViewPort = false;
            renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortDisabled.svg");

            Console.WriteLine("Generated SVG files demonstrate FitToViewPort effect.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


