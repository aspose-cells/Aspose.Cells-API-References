---
title: "Area.FillFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Area özelliği. Belirtilen grafik veya şekil için doldurma biçimlendirme özelliklerini içeren bir FillFormat nesnesini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/area/fillformat/
---
## Area.FillFormat property

Belirtilen grafik veya şekil için doldurma biçimlendirme özelliklerini içeren bir `FillFormat` nesnesini temsil eder.

```csharp
public FillFormat FillFormat { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyFillFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekle
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Bir grafik ekleyin
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Grafik veri aralığını ayarla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk serinin üçüncü noktasını alın
            ChartPoint point = chart.NSeries[0].Points[2];
            
            // Doldurma biçim özelliklerini ayarlayın
            point.Area.FillFormat.Pattern = FillPattern.DashedHorizontal;
            point.Area.FillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.Horizontal, 2);

            // Çalışma kitabını kaydedin
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FillFormat](../../fillformat/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


