---
title: "Format3D.HasTopBevelData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Format3D. Indica se la forma ha dati di smussatura superiore"
type: docs
url: /it/net/aspose.cells.drawing/format3d/hastopbeveldata/
---
## Format3D.HasTopBevelData method

Indica se la forma ha dati di smussatura superiore.

```csharp
public bool HasTopBevelData()
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class Format3DMethodHasTopBevelDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Crea un grafico 3D
            int chartIndex = sheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Ottieni il formato 3D
            Format3D format3D = chart.NSeries[0].ShapeProperties.Format3D;

            // Imposta la smussatura superiore
            format3D.TopBevel.Type = BevelPresetType.Circle;
            format3D.TopBevel.Width = 6;
            format3D.TopBevel.Height = 6;

            // Verifica e visualizza i dati di smussatura
            if (format3D.HasTopBevelData())
            {
                Console.WriteLine("Top Bevel Type: " + format3D.TopBevel.Type);
                Console.WriteLine("Top Bevel Width: " + format3D.TopBevel.Width);
                Console.WriteLine("Top Bevel Height: " + format3D.TopBevel.Height);
            }

            workbook.Save("Format3DTopBevelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


