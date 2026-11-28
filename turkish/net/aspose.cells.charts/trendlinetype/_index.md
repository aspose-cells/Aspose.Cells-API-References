---
title: "TrendlineType enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.TrendlineType enum. Trend çizgisi tipini temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/trendlinetype/
---
## TrendlineType enumeration

Trend çizgisi türünü temsil eder.

```csharp
public enum TrendlineType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Exponential | `0` | Üstel |
| Linear | `1` | Doğrusal |
| Logarithmic | `2` | Logaritmik |
| MovingAverage | `3` | Hareketli Ortalama |
| Polynomial | `4` | Polinomsal |
| Power | `5` | Güç |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineTypeDemo
    {
        public static void TrendlineTypeExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            
            // Excel nesnesine yeni bir çalışma sayfası ekleme
            int sheetIndex = workbook.Worksheets.Add();
            
            // Eklenen yeni çalışma sayfasının referansını, sayfa indeksini geçirerek elde etme
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Hücrelere örnek değerler ekleme
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Çalışma sayfasına bir grafik ekleme
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Yeni eklenen grafiğin örneğine erişme
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe, "A1" hücresinden "B4" hücresine kadar olan NSeries (grafik veri kaynağı) ekleme.
            chart.NSeries.Add("A1:B4", true);
            
            // NSeries'in kategori verileri için veri kaynağını ayarlama
            chart.NSeries.CategoryData = "C1:C4";

            // Grafiğe farklı türde trend çizgileri ekleme
            AddTrendline(chart, 0, TrendlineType.Linear, "Linear Trendline");
            AddTrendline(chart, 0, TrendlineType.Exponential, "Exponential Trendline");
            AddTrendline(chart, 0, TrendlineType.Logarithmic, "Logarithmic Trendline");
            AddTrendline(chart, 0, TrendlineType.MovingAverage, "Moving Average Trendline");
            AddTrendline(chart, 0, TrendlineType.Polynomial, "Polynomial Trendline");
            AddTrendline(chart, 0, TrendlineType.Power, "Power Trendline");

            // Excel dosyasını kaydetme
            workbook.Save("TrendlineTypeExample.xlsx");
        }

        private static void AddTrendline(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
        {
            // Belirtilen seriye belirtilen türde bir trend çizgisi ekleme
            int index = chart.NSeries[seriesIndex].TrendLines.Add(trendlineType);
            Trendline trendline = chart.NSeries[seriesIndex].TrendLines[index];
            
            // Trend çizgisinin özel adını ayarlama
            trendline.Name = trendlineName;
            
            // Grafikte denklemi gösterme
            trendline.DisplayEquation = true;
            
            // Grafikte R-Kare değerini gösterme
            trendline.DisplayRSquared = true;
            
            // Trend çizgisinin rengini ayarlama
            trendline.Color = Color.Red;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


