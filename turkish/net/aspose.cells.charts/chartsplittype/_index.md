---
title: "Enum ChartSplitType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.ChartSplitType enum. Bir pasta-pasta grafiği ya da bar-pasta grafiğinin iki bölümünün nasıl bölündüğünü temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/chartsplittype/
---
## ChartSplitType enumeration

Pie of pie grafiği ya da bar of pie grafiğinin iki bölümünün nasıl bölündüğünü temsil eder.

```csharp
public enum ChartSplitType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Position | `0` | Veri noktalarını temsil eder. Veri noktaları, ikinci grafikte veri noktalarının son bölünme konumu konularak pasta ve ikinci grafik arasında bölünecektir. |
| Value | `1` | Veri noktalarını temsil eder; değerleri Bölünme Konumundan düşük olan veri noktaları ikinci grafiğe konularak pasta ve ikinci grafik arasında bölünecektir. |
| PercentValue | `2` | Veri noktalarını temsil eder; yüzde olarak Bölünme Konumundan düşük olan noktalar ikinci grafiğe konularak pasta ve ikinci grafik arasında bölünecektir. |
| Custom | `3` | Veri noktalarını temsil eder; özel bölünme değerlerine göre pasta ve ikinci grafik arasında bölünecektir. |
| Auto | `4` | Veri noktalarını temsil eder; bu grafik türü için varsayılan mekanizma kullanılarak bölünecektir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartSplitTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Grafik için örnek veri ekleyin
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

                // Bir pasta grafiği ekle
                int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Grafik veri aralığını ayarla
                chart.NSeries.Add("B2:B5", true);
                chart.NSeries.CategoryData = "A2:A5";

                // Farklı ChartSplitType değerlerini göster
                chart.NSeries[0].SplitType = ChartSplitType.Position;
                Console.WriteLine($"Current SplitType: {chart.NSeries[0].SplitType}");

                // Başka bir bölme türüne değiştir
                chart.NSeries[0].SplitType = ChartSplitType.PercentValue;
                Console.WriteLine($"Updated SplitType: {chart.NSeries[0].SplitType}");

                // Çalışma kitabını kaydedin
                workbook.Save("ChartSplitTypeDemo.xlsx");
                Console.WriteLine("ChartSplitType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ChartSplitType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


