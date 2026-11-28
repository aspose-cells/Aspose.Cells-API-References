---
title: "ChartDataTable.HasHorizontalBorder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartDataTable özelliği. Grafik veri tablosunda yatay hücre kenarlıkları varsa True döner."
type: docs
url: /tr/net/aspose.cells.charts/chartdatatable/hashorizontalborder/
---
## ChartDataTable.HasHorizontalBorder property

Grafik veri tablosunun yatay hücre kenarları varsa doğru

```csharp
public bool HasHorizontalBorder { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasHorizontalBorderDemo
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

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Veri tablosunu etkinleştir
            chart.ShowDataTable = true;
            // Veri tablosunu ChartDataTable özelliği aracılığıyla alın
            ChartDataTable dataTable = chart.ChartDataTable;

            // HasHorizontalBorder özelliğini gösterin
            dataTable.HasHorizontalBorder = true;
            Console.WriteLine("DataTable HasHorizontalBorder: " + dataTable.HasHorizontalBorder);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartDataTablePropertyHasHorizontalBorderDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


