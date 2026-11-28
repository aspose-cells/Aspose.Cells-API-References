---
title: "PivotOptions.DropZoneSeries"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotOptions özelliği. Kaynak PivotTable'ın sütun eksenindeki her PivotTable alanı için bir kontrolün, dropZonesVisible true olarak ayarlandığında grafikte görünüp görünmeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells.charts/pivotoptions/dropzoneseries/
---
## PivotOptions.DropZoneSeries property

dropZonesVisible true olarak ayarlandığında, kaynak PivotTable'ın sütun eksenindeki her PivotTable alanı için bir denetimin grafikte görünüp görünmeyeceğini belirtir.

```csharp
public bool DropZoneSeries { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneSeriesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle ve ilk sayfayı al
            Worksheet sheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri ekle
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(7);

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("A1:B4", true);
            
            // Grafikten pivot seçeneklerini al
            PivotOptions options = chart.PivotOptions;
            
            // DropZoneSeries özelliğini göster
            Console.WriteLine("Original DropZoneSeries value: " + options.DropZoneSeries);
            options.DropZoneSeries = true;
            Console.WriteLine("Modified DropZoneSeries value: " + options.DropZoneSeries);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotOptionsPropertyDropZoneSeriesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


