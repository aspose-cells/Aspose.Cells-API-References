---
title: "Enum ChartTextDirectionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.ChartTextDirectionType enum. Grafiğin metin yönü tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/charttextdirectiontype/
---
## ChartTextDirectionType enumeration

Grafiğin metin yönü tipini temsil eder.

```csharp
public enum ChartTextDirectionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Horizontal | `0` | Yatay yön tipi. |
| Vertical | `1` | Dikey yön tipi. |
| Rotate90 | `2` | Doksan derece açıyla döndür. |
| Rotate270 | `3` | 270 derece açıyla döndür. |
| Stacked | `4` | Yığılmış metin. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartTextDirectionTypeDemo
    {
        public static void ChartTextDirectionTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafiğe veri serisi ekle
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Grafiğin başlığını ayarlayın
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Color = Color.Blue;
            
            // Grafik başlığının metin yönünü ayarla
            chart.Title.DirectionType = ChartTextDirectionType.Rotate90;
            
            // Kategori ekseni başlığının metin yönünü ayarla
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Değer ekseni başlığının metin yönünü ayarla
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.DirectionType = ChartTextDirectionType.Horizontal;
            
            // Çalışma kitabını kaydedin
            workbook.Save("ChartTextDirectionTypeExample.xlsx");
            workbook.Save("ChartTextDirectionTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


