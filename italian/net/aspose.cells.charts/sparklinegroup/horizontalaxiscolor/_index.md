---
title: "SparklineGroup.HorizontalAxisColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Ottiene e imposta il colore dell'asse orizzontale nel gruppo di sparklines"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/horizontalaxiscolor/
---
## SparklineGroup.HorizontalAxisColor property

Ottiene e imposta il colore dell'asse orizzontale nel gruppo di sparkline.

```csharp
public CellsColor HorizontalAxisColor { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyHorizontalAxisColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(4);

            // Crea gruppo sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Imposta il colore dell'asse orizzontale
            CellsColor axisColor = workbook.CreateCellsColor();
            axisColor.Color = Color.Blue;
            group.HorizontalAxisColor = axisColor;
            group.ShowHorizontalAxis = true;

            // Salva la cartella di lavoro
            workbook.Save("SparklineHorizontalAxisColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


