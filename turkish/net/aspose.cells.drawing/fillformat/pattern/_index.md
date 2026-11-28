---
title: "FillFormat.Pattern"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FillFormat özelliği. Bir alanın görüntüleme desenini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/fillformat/pattern/
---
## FillFormat.Pattern property

Bir alanın görüntü desenini temsil eder.

```csharp
public FillPattern Pattern { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPatternDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue(50);
            sheet.Cells["A2"].PutValue(100);
            sheet.Cells["A3"].PutValue(150);

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("A1:A3", true);

            // İlk seriye ve onun ilk noktasına eriş
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Noktanın alanı için doldurma desenini ayarla
            point.Area.FillFormat.Pattern = FillPattern.DottedGrid;
            
            // Çalışma kitabını kaydedin
            workbook.Save("FillFormatPatternDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


