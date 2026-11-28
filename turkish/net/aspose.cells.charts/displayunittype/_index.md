---
title: "Enum DisplayUnitType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.DisplayUnitType enum. Grafik ekseninin görüntü birimi türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/displayunittype/
---
## DisplayUnitType enumeration

Grafik ekseninin görüntü birimi tipini temsil eder.

```csharp
public enum DisplayUnitType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Görüntü birimi Yok. |
| Hundreds | `1` | Grafikteki değerlerin 100 ile bölüneceğini belirtir. |
| Thousands | `2` | Grafikteki değerlerin 1.000 ile bölüneceğini belirtir. |
| TenThousands | `3` | Grafikteki değerlerin 10.000 ile bölüneceğini belirtir. |
| HundredThousands | `4` | Grafikteki değerlerin 100.000 ile bölüneceğini belirtir. |
| Millions | `5` | Grafikteki değerlerin 1.000.000 ile bölüneceğini belirtir. |
| TenMillions | `6` | Grafikteki değerlerin 10.000.000 ile bölüneceğini belirtir. |
| HundredMillions | `7` | Grafikteki değerlerin 100.000.000 ile bölüneceğini belirtir. |
| Billions | `8` | Grafikteki değerlerin 1.000.000.000 ile bölüneceğini belirtir. |
| Trillions | `9` | Grafikteki değerlerin 1.000.000.000.000 ile bölüneceğini belirtir. |
| Percentage | `10` | Grafikteki değerler 0,01 ile bölünecektir. |
| Cust | `11` | Görüntü birimi için özel bir değer belirtir. |
| Custom | `12` | Görüntü birimi için özel bir değer belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitTypeDemo
    {
        public static void DisplayUnitTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabına yeni bir çalışma sayfası ekle
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Çalışma sayfasına bazı örnek veriler ekleyin
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe "A1" hücresinden "B3" hücresine kadar uzanan NSeries (grafik veri kaynağı) ekleyin
            chart.NSeries.Add("A1:B3", true);
            
            // Değer ekseninin görüntü birimini Milyon olarak ayarlayın
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            
            // İsteğe bağlı olarak, görüntü birimi etiketini göster
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("DisplayUnitTypeExample.xlsx");
            workbook.Save("DisplayUnitTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


