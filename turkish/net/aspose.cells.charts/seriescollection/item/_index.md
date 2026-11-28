---
title: "SeriesCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesCollection özelliği. Belirtilen dizindeki Series öğesini alır"
type: docs
url: /tr/net/aspose.cells.charts/seriescollection/item/
---
## SeriesCollection indexer

Belirtilen dizindeki [`Series`](../../series/) öğesini alır.

```csharp
public Series this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("Series");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Values");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Item özelliğini kullanarak ilk seriye ve onun ilk noktasına erişin
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            // Nokta görünümünü özelleştir
            point.Area.FillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.White, GradientStyleType.Vertical, 2);
            point.Area.FillFormat.FillType = FillType.Solid;

            // Çalışma kitabını kaydedin
            workbook.Save("SeriesCollectionPropertyItemDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


