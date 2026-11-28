---
title: "PptxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PptxSaveOptions özelliği. Bir xlsx dosyasının grafik veri kaynağı olarak gömülüp gömülmediğini gösterir."
type: docs
url: /tr/net/aspose.cells/pptxsaveoptions/embedxlsxaschartdatasource/
---
## PptxSaveOptions.EmbedXlsxAsChartDataSource property

Grafiğin veri kaynağı olarak bir xlsx dosyasının gömülüp gömülmediğini gösterir.

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### Açıklamalar

Varsayılan değer true'tur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PptxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Grafik verileriyle örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Özelliğin etkisini göstermek için bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // PptxSaveOptions örneği oluşturun
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // EmbedXlsxAsChartDataSource'un varsayılan değerini gösterin
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Özelliği true olarak ayarlayarak kullanımını gösterin
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Seçenek etkinleştirilmiş şekilde çalışma kitabını PPTX olarak kaydedin
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with EmbedXlsxAsChartDataSource enabled");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


