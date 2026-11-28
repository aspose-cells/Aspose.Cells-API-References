---
title: "Cells.FirstCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Bu çalışma sayfasındaki ilk hücreyi alır"
type: docs
url: /tr/net/aspose.cells/cells/firstcell/
---
## Cells.FirstCell property

Bu çalışma sayfasındaki ilk hücreyi alır.

```csharp
public Cell FirstCell { get; }
```

### Açıklamalar

Çalışma sayfasında veri yoksa null döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class CellsPropertyFirstCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(2000);
            
            // Hücre koleksiyonunu al
            Cells cells = worksheet.Cells;
            
            // FirstCell özelliğini göster
            Cell firstCell = cells.FirstCell;
            Console.WriteLine($"First cell address: {firstCell.Name}");
            Console.WriteLine($"First cell value: {firstCell.Value}");
            
            // FirstCell ve LastCell kullanarak grafik oluştur
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange($"{cells.FirstCell.Name}:{cells.LastCell.Name}", true);
            chart.ShowLegend = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("FirstCellDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


