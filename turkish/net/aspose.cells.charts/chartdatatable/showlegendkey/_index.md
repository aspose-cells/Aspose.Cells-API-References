---
title: "ChartDataTable.ShowLegendKey"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartDataTable özelliği. Veri etiketi lejand anahtarı görünürse true"
type: docs
url: /tr/net/aspose.cells.charts/chartdatatable/showlegendkey/
---
## ChartDataTable.ShowLegendKey property

Veri etiketi açıklama anahtarı görünürse doğru.

```csharp
public bool ShowLegendKey { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyShowLegendKeyDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Lejand anahtarıyla veri tablosunu etkinleştir
            chart.ShowDataTable = true;
            // Chart'ın özellikleri aracılığıyla DataTable'a erişin
            if (chart.ChartDataTable != null)
            {
                chart.ChartDataTable.ShowLegendKey = true;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ChartDataTableShowLegendKeyDemo.xlsx");

            Console.WriteLine("Chart created with ShowLegendKey enabled in data table.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


