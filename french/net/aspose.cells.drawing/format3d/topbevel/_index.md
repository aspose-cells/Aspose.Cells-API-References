---
title: "Format3D.TopBevel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Format3D. Obtient l'objet Bevel qui contient les propriétés associées à la définition d'un chanfrein sur la face supérieure ou avant d'une forme"
type: docs
url: /fr/net/aspose.cells.drawing/format3d/topbevel/
---
## Format3D.TopBevel property

Obtient l'objet [`Bevel`](../../bevel/) qui contient les propriétés associées à la définition d'un chanfrein sur la face supérieure ou avant d'une forme.

```csharp
public Bevel TopBevel { get; }
```

### Exemples

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

### Voir aussi

* class [Bevel](../../bevel/)
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


