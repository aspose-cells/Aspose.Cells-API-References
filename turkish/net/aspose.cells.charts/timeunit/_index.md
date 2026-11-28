---
title: "Enum TimeUnit"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.TimeUnit enum. Kategori ekseni için temel birimi temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/timeunit/
---
## TimeUnit enumeration

Kategori ekseni için temel birimi temsil eder.

```csharp
public enum TimeUnit
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Days | `0` | Günler |
| Months | `1` | Aylar |
| Years | `2` | Yıllar |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TimeUnitDemo
    {
        public static void TimeUnitExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // Yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["B3"].PutValue(300);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe seri ekle
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Kategori eksenini zaman birimlerini kullanacak şekilde ayarlayın
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.CategoryType = CategoryType.TimeScale;
            categoryAxis.BaseUnitScale = TimeUnit.Months;
            categoryAxis.MajorUnitScale = TimeUnit.Months;
            categoryAxis.MinorUnitScale = TimeUnit.Days;

            // Grafiğin görünümünü özelleştirin
            chart.Title.Text = "Sample Chart with Time Units";
            chart.ValueAxis.Title.Text = "Values";
            chart.CategoryAxis.Title.Text = "Dates";

            // Çalışma kitabını kaydedin
            workbook.Save("TimeUnitExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


