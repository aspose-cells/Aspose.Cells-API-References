---
title: "ChartPointCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartPointCollection özelliği. Seride belirtilen indeksteki ChartPoint öğesini alır"
type: docs
url: /tr/net/aspose.cells.charts/chartpointcollection/item/
---
## ChartPointCollection indexer

Belirtilen indeksteki serideki [`ChartPoint`](../../chartpoint/) öğesini alır.

```csharp
public ChartPoint this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Serideki grafik noktasının indeksi. |

### Dönüş Değeri

ChartPoint nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Item özelliğini kullanarak belirli bir grafik noktasına erişin
            ChartPoint point = chart.NSeries[0].Points[1];
            
            // Noktanın dolgu desenini değiştirin
            point.Area.FillFormat.Pattern = FillPattern.LightHorizontal;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartPoint](../../chartpoint/)
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


