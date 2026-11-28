---
title: "Area.InvertIfNegative"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Area özelliği. Özellik true ise ve grafik noktasının değeri negatif bir sayı ise ön plan rengi ve arka plan rengi değiştirilecektir"
type: docs
url: /tr/net/aspose.cells.drawing/area/invertifnegative/
---
## Area.InvertIfNegative property

Özellik true ise ve grafik noktasının değeri negatif bir sayı ise, ön plan rengi ve arka plan rengi değiştirilecektir.

```csharp
public bool InvertIfNegative { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyInvertIfNegativeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Negatif değerli örnek veri ekleyin
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Sütun grafik ekle
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Veri serileri ekleyin ve alan özelliklerini yapılandırın
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Area.InvertIfNegative = true;
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.BackgroundColor = Color.Yellow;
            
            workbook.Save("AreaPropertyInvertIfNegativeDemo.xls");
        }
    }
}
```

### Ayrıca Bakınız

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


