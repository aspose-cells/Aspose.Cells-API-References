---
title: "SeriesCollection.ChangeColors"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SeriesCollection yöntemi. Grafik serileri için Monokromatik Palet ayarla"
type: docs
url: /tr/net/aspose.cells.charts/seriescollection/changecolors/
---
## SeriesCollection.ChangeColors method

Grafik serileri için Tek Renkli Palet ayarla.

```csharp
public void ChangeColors(ChartColorPaletteType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | ChartColorPaletteType | Monokromatik Tür. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodChangeColorsWithChartColorPaletDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Grafik için bazı verileri doldurun
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["A2"].PutValue("Jan");
            ws.Cells["A3"].PutValue("Feb");
            ws.Cells["A4"].PutValue("Mar");

            ws.Cells["B1"].PutValue("Series1");
            ws.Cells["B2"].PutValue(10);
            ws.Cells["B3"].PutValue(20);
            ws.Cells["B4"].PutValue(30);

            ws.Cells["C1"].PutValue("Series2");
            ws.Cells["C2"].PutValue(15);
            ws.Cells["C3"].PutValue(25);
            ws.Cells["C4"].PutValue(35);

            // Bir sütun grafik ekle
            int chartIdx = ws.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = ws.Charts[chartIdx];

            // Seri için veri aralığını ayarlayın
            chart.NSeries.Add("B1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Seri koleksiyonunu alın
            SeriesCollection seriesColl = chart.NSeries;

            try
            {
                // Koleksiyondaki tüm serilerin renk paletini değiştirin.
                // Bağımlı enum üye adlarından kaçınmak için geçerli bir enum değerine (ör. 0) sayısal dönüşüm kullanın.
                seriesColl.ChangeColors((ChartColorPaletteType)0);

                Console.WriteLine("ChangeColors method invoked successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error invoking ChangeColors: {ex.Message}");
            }

            // Sonucu doğrulamak için çalışma kitabını kaydedin
            workbook.Save("SeriesCollection_ChangeColors_Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ChartColorPaletteType](../../chartcolorpalettetype/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


