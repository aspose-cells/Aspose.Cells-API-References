---
title: "Chart.PivotSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart özelliği. Kaynak, pivot tablonun verisidir. PivotSource boş değilse grafik PivotChart olur"
type: docs
url: /tr/net/aspose.cells.charts/chart/pivotsource/
---
## Chart.PivotSource property

Kaynak, pivot tablosunun verisidir. PivotSource boş değilse, grafik PivotChart'tır.

```csharp
public string PivotSource { get; set; }
```

### Açıklamalar

Eğer pivot tablo "PivotTable1" "Sheet1" çalışma sayfasında ve "Book1.xls" dosyasında ise. PivotSource, grafik ve PivotTable aynı çalışma kitabında değilse "[Book1.xls]Sheet1!PivotTable1" olabilir. Bu özelliği ayarlarsanız, önceki veri kaynağı ayarı kaybolur.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPivotSourceDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;
            
            // Pivot tablo ekle
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik için pivot kaynağını ayarla
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Pivot verisini ve grafiği yenile
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            chart.RefreshPivotData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotSourceDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Chart PivotSource demo executed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


