---
title: "Line.IsAutomaticColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Line özelliği. Çizgi renginin otomatik atanıp atanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/line/isautomaticcolor/
---
## Line.IsAutomaticColor property

Çizgi renginin otomatik atanıp atanmadığını gösterir.

```csharp
public bool IsAutomaticColor { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LinePropertyIsAutomaticColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir grafik için örnek veri ekle
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

                // IsAutomaticColor özelliği değerini okuyun ve gösterin
                Console.WriteLine("IsAutomaticColor value: " + seriesLine.IsAutomaticColor);

                // Çalışma kitabını kaydedin
                workbook.Save("IsAutomaticColorDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


