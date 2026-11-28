---
title: "Enum ErrorBarType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.ErrorBarType enum. Hata çubuğu miktar türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/errorbartype/
---
## ErrorBarType enumeration

Hata çubuğu miktar tipini temsil eder.

```csharp
public enum ErrorBarType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Custom | `0` | InnerCustom değer türü. |
| FixedValue | `1` | Sabit değer türü. |
| Percent | `2` | Yüzde türü |
| StDev | `3` | Standart sapma türü. |
| StError | `4` | Standart hata türü. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarTypeDemo
    {
        public static void ErrorBarTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Örnek veri ekleyin
            cells["A1"].PutValue(2);
            cells["A2"].PutValue(5);
            cells["A3"].PutValue(3);
            cells["A4"].PutValue(6);
            cells["B1"].PutValue(4);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(6);
            cells["B4"].PutValue(7);

            cells["C1"].PutValue("Q1");
            cells["C2"].PutValue("Q2");
            cells["C3"].PutValue("Y1");
            cells["C4"].PutValue("Y2");

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Grafikteki her seri için hata çubuğu özelliklerini ayarla
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ErrorBarTypeExample.xlsx");
            workbook.Save("ErrorBarTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


