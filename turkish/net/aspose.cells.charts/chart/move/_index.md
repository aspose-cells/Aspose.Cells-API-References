---
title: "Chart.Move"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart yöntemi. Grafiği belirtilen konuma taşır"
type: docs
url: /tr/net/aspose.cells.charts/chart/move/
---
## Chart.Move method

Grafiği belirtilen konuma taşır.

```csharp
public void Move(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| topRow | Int32 | Sol üst satır indeksi. |
| rightColumn | Int32 | Alt sağ sütun indeksi |
| bottomRow | Int32 | Alt sağ satır indeksi |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodMoveWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Orijinal grafik konumu
                Console.WriteLine($"Original position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Grafiği yeni konuma taşı (satırlar 10-20, sütunlar 2-8)
                chart.Move(10, 2, 20, 8);

                // Yeni konumu göster
                Console.WriteLine($"New position - topRow: {chart.ChartObject.UpperLeftRow}, leftColumn: {chart.ChartObject.UpperLeftColumn}");

                // Çalışma kitabını kaydedin
                workbook.Save("ChartMoveDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Move method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


