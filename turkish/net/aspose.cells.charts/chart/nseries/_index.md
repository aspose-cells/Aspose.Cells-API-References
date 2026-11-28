---
title: "Chart.NSeries"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Grafikteki veri serilerini temsil eden bir SeriesCollection koleksiyonu alır"
type: docs
url: /tr/net/aspose.cells.charts/chart/nseries/
---
## Chart.NSeries property

Grafikteki veri serilerini temsil eden bir [`SeriesCollection`](../../seriescollection/) koleksiyonu alır.

```csharp
public SeriesCollection NSeries { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyNSeriesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 2, 25, 11);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            // NSeries kullanarak grafik serileri için veri kaynağını ayarla
            chart.NSeries.Add("=Sheet1!$A$2:$B$10", true);

            // Grafik başlığını ayarla
            chart.Title.Text = "NSeries Demo Chart";

            // Çalışma kitabını kaydedin
            workbook.Save("NSeriesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


