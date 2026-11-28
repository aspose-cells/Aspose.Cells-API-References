---
title: "Enum PlotDataByType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.PlotDataByType enum. Satır veya sütun bazında veri grafiği tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/plotdatabytype/
---
## PlotDataByType enumeration

Veri grafiğinin satır veya sütun bazında türünü temsil eder.

```csharp
public enum PlotDataByType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Row | `0` | Satıra göre sıralanmış. |
| Column | `1` | Sütuna göre. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassPlotDataByTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Çalışma sayfasına örnek veri ekle
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value1");
                worksheet.Cells["C1"].PutValue("Value2");
                worksheet.Cells["A2"].PutValue("Row1");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["C2"].PutValue(20);
                worksheet.Cells["A3"].PutValue("Row2");
                worksheet.Cells["B3"].PutValue(30);
                worksheet.Cells["C3"].PutValue(40);

                // Çalışma sayfasına bir grafik ekleyin
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Grafik veri aralığını ayarla
                chart.NSeries.Add("B2:C3", true);

                // PlotDataByType enum değerlerini kullanmayı göster
                PlotDataByType plotType = PlotDataByType.Row;
                Console.WriteLine($"Chart is currently plotting data by: {plotType}");

                // Sütuna göre çizime değiştir
                plotType = PlotDataByType.Column;
                Console.WriteLine($"Chart is now plotting data by: {plotType}");

                // Çalışma kitabını kaydedin
                workbook.Save("PlotDataByTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with PlotDataByType demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PlotDataByType: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


