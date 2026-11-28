---
title: "Enum BubbleSizeRepresents"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.BubbleSizeRepresents enum. Balon boyutunun bir balon grafiğinde neyi temsil ettiğini gösterir."
type: docs
url: /tr/net/aspose.cells.charts/bubblesizerepresents/
---
## BubbleSizeRepresents enumeration

Balon grafiğinde balon boyutunun neyi temsil ettiğini temsil eder.

```csharp
public enum BubbleSizeRepresents
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| SizeIsArea | `0` | Balonun alanı olan [`BubbleSizes`](../series/bubblesizes/) değerini temsil eder. |
| SizeIsWidth | `1` | `[`BubbleSizes`](../series/bubblesizes/)` değerini temsil eder; balonun genişliğidir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class BubbleSizeRepresentsDemo
    {
        public static void BubbleSizeRepresentsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Balon grafiği için örnek veri ekle
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            // Çalışma sayfasına bir balon grafiği ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Balon grafiğine seri ekle
            int seriesIndex = chart.NSeries.Add("A1:C3", true);
            Series series = chart.NSeries[seriesIndex];

            // X değerlerini, Y değerlerini ve balon boyutlarını ayarla
            series.XValues = "A1:A3";
            series.Values = "B1:B3";
            series.BubbleSizes = "C1:C3";

            // Balon boyutu temsilini ayarla
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // Çalışma kitabını kaydedin
            workbook.Save("BubbleSizeRepresentsExample.xlsx");
            workbook.Save("BubbleSizeRepresentsExample.pdf");

            // Balon boyutu temsilini ayarla
            series.SizeRepresents = BubbleSizeRepresents.SizeIsWidth;

            // Çalışma kitabını kaydedin
            workbook.Save("BubbleSizeRepresentsExample2.xlsx");
            workbook.Save("BubbleSizeRepresentsExample2.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


