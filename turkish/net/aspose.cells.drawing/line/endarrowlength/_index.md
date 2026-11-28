---
title: "Line.EndArrowLength"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Line özelliği. Çizginin ucundaki ok başının uzunluğunu belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/line/endarrowlength/
---
## Line.EndArrowLength property

Bir çizginin sonu için ok başının uzunluğunu belirtir.

```csharp
public MsoArrowheadLength EndArrowLength { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyEndArrowLengthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(40);

            try
            {
                // Çizgi özelliklerini göstermek için bir grafik ekleyin
                int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 15, 5);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B3", true);

                // Grafik serisi kenarından çizgi özelliklerini al
                Line line = chart.NSeries[0].Border;

                // EndArrowLength'i göstermek için bir ok ucu tipi ayarlayın
                line.EndType = MsoArrowheadStyle.Arrow;

                // Mevcut EndArrowLength değerini gösterin
                Console.WriteLine("Current EndArrowLength: " + line.EndArrowLength);

                // Yeni bir EndArrowLength değeri ayarlayın
                line.EndArrowLength = MsoArrowheadLength.Long;
                Console.WriteLine("Updated EndArrowLength: " + line.EndArrowLength);

                // Çalışma kitabını kaydedin
                workbook.Save("EndArrowLengthDemo.xlsx");
                Console.WriteLine("EndArrowLength property demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


