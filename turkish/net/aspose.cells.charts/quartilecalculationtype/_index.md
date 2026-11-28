---
title: "Enum QuartileCalculationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.QuartileCalculationType enum. Çeyrek hesaplama yöntemlerini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/quartilecalculationtype/
---
## QuartileCalculationType enumeration

Çeyrek hesaplama yöntemlerini temsil eder.

```csharp
public enum QuartileCalculationType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Exclusive | `0` | Çeyrek hesaplaması, veri kümesini çeyreklerine ayırırken medyanı içerir. |
| Inclusive | `1` | Çeyrek hesaplaması, veri kümesini çeyreklerine ayırırken medyanı dışarı bırakır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class QuartileCalculationTypeDemo
    {
        public static void QuartileCalculationTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafiğe seri ekle
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Seri düzen özelliklerine erişin
            SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;

            // Çeyrek hesaplama türünü ayarlayın
            layoutProperties.QuartileCalculation = QuartileCalculationType.Exclusive;

            // Çalışma kitabını kaydedin
            workbook.Save("QuartileCalculationTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


