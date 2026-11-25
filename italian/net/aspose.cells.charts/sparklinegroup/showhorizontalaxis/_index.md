---
title: "SparklineGroup.ShowHorizontalAxis"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Indica se mostrare l'asse orizzontale della sparkline. L'asse orizzontale appare se la sparkline ha dati che attraversano l'asse zero"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/showhorizontalaxis/
---
## SparklineGroup.ShowHorizontalAxis property

Indica se mostrare l'asse orizzontale della sparkline. L'asse orizzontale appare se la sparkline ha dati che attraversano l'asse zero.

```csharp
public bool ShowHorizontalAxis { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowHorizontalAxisDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definisci la posizione dello sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Aggiungi gruppo di sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Configura le proprietà delle sparklines
            group.ShowHorizontalAxis = true;
            CellsColor axisColor = workbook.CreateCellsColor();
            axisColor.Color = Color.Gray;
            group.HorizontalAxisColor = axisColor;

            // Salva la cartella di lavoro
            workbook.Save("SparklineWithHorizontalAxis.xlsx");
        }
    }
}
```

### Vedi anche

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


