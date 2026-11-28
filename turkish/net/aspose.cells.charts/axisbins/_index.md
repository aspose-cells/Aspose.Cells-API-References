---
title: "Sınıf AxisBins"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.AxisBins sınıfı. Eksen kutularını temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/axisbins/
---
## AxisBins class

Eksen kutularını temsil eder

```csharp
public class AxisBins
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.cells.charts/axisbins/count/) { get; set; } | Eksen kutularının sayısını alır veya ayarlar |
| [IsAutomatic](../../aspose.cells.charts/axisbins/isautomatic/) { get; set; } | Eksen kutularının otomatik olup olmadığını gösterir. |
| [IsByCategory](../../aspose.cells.charts/axisbins/isbycategory/) { get; set; } | Verileri kategoriye göre gruplandırmanın etkin olup olmadığını gösterir. |
| [Overflow](../../aspose.cells.charts/axisbins/overflow/) { get; set; } | Eksen kutularının taşmasını alır veya ayarlar |
| [Underflow](../../aspose.cells.charts/axisbins/underflow/) { get; set; } | Eksen kutularının eksik akışını alır veya ayarlar |
| [Width](../../aspose.cells.charts/axisbins/width/) { get; set; } | Eksen kutusunun genişliğini alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [ResetOverflow](../../aspose.cells.charts/axisbins/resetoverflow/)() | (**Obsolete.**) Taşmayı sıfırla |
| [ResetUnderflow](../../aspose.cells.charts/axisbins/resetunderflow/)() | (**Obsolete.**) Eksik akışı sıfırla |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsDemo
    {
        public static void AxisBinsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // Yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe veri serisi ekle
            chart.NSeries.Add("A1:A5", true);

            // Değer eksenine erişin
            Axis valueAxis = chart.ValueAxis;

            // Değer ekseninin kutularına erişin
            AxisBins bins = valueAxis.Bins;

            // Kutular için özellikleri ayarlayın
            bins.IsByCategory = false;
            bins.IsAutomatic = true;
            bins.Width = 10.0;
            bins.Count = 5;
            bins.Overflow = 60.0;
            bins.Underflow = 0.0;

            // Taşma ve eksik akışı sıfırla
            //bins.ResetOverflow();
            //bins.ResetUnderflow();

            // Çalışma kitabını kaydedin
            workbook.Save("AxisBinsExample.xlsx");
            workbook.Save("AxisBinsExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


