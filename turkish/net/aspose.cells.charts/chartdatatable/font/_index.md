---
title: "ChartDataTable.Font"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartDataTable özelliği. Belirtilen grafik veri tablosunun yazı tipi ayarını temsil eden bir Font nesnesi alır"
type: docs
url: /tr/net/aspose.cells.charts/chartdatatable/font/
---
## ChartDataTable.Font property

`Font` nesnesi alır; bu nesne belirtilen grafik veri tablosunun yazı tipi ayarını temsil eder.

```csharp
public Font Font { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyFontDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Veri tablosunu etkinleştir
            chart.ShowDataTable = true;
            
            // Veri tablosu nesnesini al
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Veri tablosu yazı tipini özelleştir
            dataTable.Font.Size = 14;
            dataTable.Font.Color = Color.Red;
            dataTable.Font.IsBold = true;
            dataTable.Font.Name = "Arial";

            // Çalışma kitabını kaydedin
            workbook.Save("ChartDataTableFontDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../../../aspose.cells/font/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


