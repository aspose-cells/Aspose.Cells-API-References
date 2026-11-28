---
title: "Line.BeginArrowLength"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Line özelliği. Bir çizginin başlangıcı için ok başının uzunluğunu belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/line/beginarrowlength/
---
## Line.BeginArrowLength property

Bir çizginin başlangıcı için ok başının uzunluğunu belirtir.

```csharp
public MsoArrowheadLength BeginArrowLength { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class LinePropertyBeginArrowLengthDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir grafik için basit verileri hazırlayın
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Bir çizgi grafik ekle
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // İlk serinin çizgi (kenar) özelliğine erişin
                Line seriesLine = chart.NSeries[0].Border;

                // BeginArrowLength değerini Uzun olarak ayarlayın
                seriesLine.BeginArrowLength = MsoArrowheadLength.Long;

                // Mevcut BeginArrowLength değerini okuyun ve görüntüleyin
                Console.WriteLine("BeginArrowLength value: " + seriesLine.BeginArrowLength);

                // Çalışma kitabını kaydedin (isteğe bağlı, sadece demoyu tamamlamak için).
                workbook.Save("BeginArrowLengthDemo.xlsx");
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


