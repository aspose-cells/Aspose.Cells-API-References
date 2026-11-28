---
title: "Line.IsAuto"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Line özelliği. Bu çizgi stilinin otomatik atanıp atanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/line/isauto/
---
## Line.IsAuto property

Bu çizgi stilinin otomatik atanıp atanmadığını gösterir.

```csharp
public bool IsAuto { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyIsAutoDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Bir çizgi grafik ekle
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

                // Grafik veri aralığını ayarla
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Serinin çizgi özelliklerine erişin
                Aspose.Cells.Charts.Series series = chart.NSeries[0];
                Line line = series.Border;

                // Mevcut IsAuto değerini gösterin
                Console.WriteLine("Initial IsAuto value: " + line.IsAuto);

                // IsAuto'yi true olarak ayarlayın
                line.IsAuto = true;
                Console.WriteLine("After setting to true, IsAuto value: " + line.IsAuto);

                // IsAuto'yi false olarak ayarlayın
                line.IsAuto = false;
                Console.WriteLine("After setting to false, IsAuto value: " + line.IsAuto);

                // Çalışma kitabını kaydedin
                workbook.Save("IsAutoDemo.xlsx");
                Console.WriteLine("IsAuto property has been demonstrated successfully.");
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

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


