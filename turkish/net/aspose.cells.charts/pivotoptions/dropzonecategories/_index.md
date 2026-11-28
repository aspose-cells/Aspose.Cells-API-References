---
title: "PivotOptions.DropZoneCategories"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotOptions özelliği. Kaynak PivotTable'ın satır eksenindeki her PivotTable alanı için bir kontrolün, dropZonesVisible true olarak ayarlandığında grafikte görünüp görünmeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells.charts/pivotoptions/dropzonecategories/
---
## PivotOptions.DropZoneCategories property

dropZonesVisible true olarak ayarlandığında, kaynak PivotTable'ın satır eksenindeki her PivotTable alanı için bir denetimin grafikte görünüp görünmeyeceğini belirtir.

```csharp
public bool DropZoneCategories { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneCategoriesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ve bazı örnek veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // Pivot verilerini kullanan bir grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Grafikten pivot seçeneklerine eriş
            PivotOptions options = chart.PivotOptions;
            
            // DropZoneCategories özelliğini göster
            options.DropZoneCategories = true;
            Console.WriteLine("DropZoneCategories enabled: " + options.DropZoneCategories);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotOptionsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


