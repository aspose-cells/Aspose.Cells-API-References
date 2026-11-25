---
title: "SparklineGroup.ShowNegativePoints"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Indica se evidenziare i valori negativi nel gruppo sparkline con un colore o un marcatore diverso"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/shownegativepoints/
---
## SparklineGroup.ShowNegativePoints property

Indica se evidenziare i valori negativi nel gruppo di sparkline con un colore o un marcatore diverso.

```csharp
public bool ShowNegativePoints { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowNegativePointsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati con valori negativi per dimostrare ShowNegativePoints
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(-2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(-3);

            // Definisci il CellArea per lo sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Aggiungi un gruppo sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Configura le proprietà del gruppo sparkline
            group.ShowNegativePoints = true;
            CellsColor negativePointsColor = workbook.CreateCellsColor();
            negativePointsColor.Color = Color.Blue;
            group.NegativePointsColor = negativePointsColor;

            // Salva la cartella di lavoro
            workbook.Save("SparklineNegativePointsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


