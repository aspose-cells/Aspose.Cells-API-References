---
title: "SparklineGroup.PlotEmptyCellsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroup. Indique comment tracer les cellules vides"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/plotemptycellstype/
---
## SparklineGroup.PlotEmptyCellsType property

Indique comment tracer les cellules vides.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPlotEmptyCellsTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données avec quelques cellules vides
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(null); // Empty cell
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Définit la CellArea pour le sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Ajouter un groupe de sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Définir comment les cellules vides doivent être tracées
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;

            // Ajouter un sparkline au groupe
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Enregistrez le classeur
            workbook.Save("SparklineEmptyCellsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


