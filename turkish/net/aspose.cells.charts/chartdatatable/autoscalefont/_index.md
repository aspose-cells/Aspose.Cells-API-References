---
title: "ChartDataTable.AutoScaleFont"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartDataTable özelliği. Nesnenin boyutu değiştiğinde metnin yazı tipi boyutunu değiştirmesi durumunda doğru. Varsayılan değer True'dur"
type: docs
url: /tr/net/aspose.cells.charts/chartdatatable/autoscalefont/
---
## ChartDataTable.AutoScaleFont property

Nesnedeki metin, nesne boyutu değiştiğinde yazı tipi boyutunu değiştiriyorsa True döner. Varsayılan değer True'dur.

```csharp
public bool AutoScaleFont { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyAutoScaleFontDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Chart veri kaynağını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Veri tablosunu etkinleştir
            chart.ShowDataTable = true;
            
            // Chart veri tablosu özelliklerine erişin
            // ShowDataTable true olduğunda ChartDataTable'ı almanın doğru yolu
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // AutoScaleFont özelliğini göster
            dataTable.AutoScaleFont = false; // Disable auto-scaling
            Console.WriteLine("AutoScaleFont (false): " + dataTable.AutoScaleFont);
            
            dataTable.AutoScaleFont = true; // Enable auto-scaling
            Console.WriteLine("AutoScaleFont (true): " + dataTable.AutoScaleFont);

            // Çalışma kitabını kaydedin
            workbook.Save("ChartDataTableAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


