---
title: "SparklineGroup.ShowHighPoint"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Indica se evidenziare i punti più alti dei dati nel gruppo sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/showhighpoint/
---
## SparklineGroup.ShowHighPoint property

Indica se evidenziare i punti più alti dei dati nel gruppo di sparkline.

```csharp
public bool ShowHighPoint { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowHighPointDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Crea gruppo sparkline
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Aggiungi sparkline
            group.Sparklines.Add("A1:D1", 0, 4);

            // Configura la visualizzazione dei punti più alti
            group.ShowHighPoint = true;
            CellsColor highColor = workbook.CreateCellsColor();
            highColor.Color = System.Drawing.Color.Green;
            group.HighPointColor = highColor;

            // Salva cartella di lavoro
            workbook.Save("SparklineHighPointDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


