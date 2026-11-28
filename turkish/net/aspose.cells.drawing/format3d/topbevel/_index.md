---
title: "Format3D.TopBevel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Format3D özelliği. Şeklin üst veya ön yüzünde bir köşe (bevel) tanımlamaya ilişkin özellikleri tutan Bevel nesnesini alır"
type: docs
url: /tr/net/aspose.cells.drawing/format3d/topbevel/
---
## Format3D.TopBevel property

[`Bevel`](../../bevel/) nesnesini alır; bu nesne, şeklin üst veya ön yüzünde bir köşe (bevel) tanımlamaya ilişkin özellikleri tutar.

```csharp
public Bevel TopBevel { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class Format3DPropertyTopBevelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            Series series = chart.NSeries[0];
            Format3D format3D = series.ShapeProperties.Format3D;

            try
            {
                Bevel topBevel = format3D.TopBevel;
                Console.WriteLine("TopBevel Width: " + topBevel.Width);
                Console.WriteLine("TopBevel Height: " + topBevel.Height);
                Console.WriteLine("TopBevel Type: " + topBevel.Type);

                if (format3D.HasTopBevelData())
                {
                    Console.WriteLine("Shape has top bevel data");
                }
                else
                {
                    Console.WriteLine("Shape does not have top bevel data");
                }

                workbook.Save("TopBevelDemo.xlsx");
                Console.WriteLine("TopBevel properties displayed successfully.");
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

* class [Bevel](../../bevel/)
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


