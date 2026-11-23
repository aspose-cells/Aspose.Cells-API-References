---
title: "SparklineGroup.Sparklines"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroup. Obtient la collection d'objets Sparkline"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/sparklines/
---
## SparklineGroup.Sparklines property

Obtient la collection d'objets [`Sparkline`](../../sparkline/).

```csharp
public SparklineCollection Sparklines { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertySparklinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Créer un groupe de sparkline
            CellArea location = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 4, EndColumn = 4 };
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Ajouter un sparkline en utilisant la propriété Sparklines
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Personnaliser l'apparence du sparkline
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // Enregistrez le classeur
            workbook.Save("SparklineDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


