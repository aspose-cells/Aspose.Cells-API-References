---
title: "Chart.SubTitle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Grafiğin alt başlığını alır. Yalnızca ODS dosyalarına uygulanır"
type: docs
url: /tr/net/aspose.cells.charts/chart/subtitle/
---
## Chart.SubTitle property

Grafiğin alt başlığını alır. Yalnızca ODS dosyalarına uygulanır.

```csharp
public Title SubTitle { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySubTitleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin ve veri aralığını ayarlayın
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ana başlığı ayarlayın
            chart.Title.Text = "Main Chart Title";

            // Alt başlığı ayarlayın
            chart.SubTitle.Text = "Chart Subtitle";
            chart.SubTitle.Font.Size = 12;
            chart.SubTitle.Font.IsBold = true;

            // Çalışma kitabını kaydedin
            workbook.Save("ChartWithSubtitle.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Title](../../title/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


