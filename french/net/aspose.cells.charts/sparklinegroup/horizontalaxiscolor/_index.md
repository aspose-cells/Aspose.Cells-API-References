---
title: "SparklineGroup.HorizontalAxisColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroup. Obtient et définit la couleur de l'axe horizontal dans le groupe de sparklines"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/horizontalaxiscolor/
---
## SparklineGroup.HorizontalAxisColor property

Obtient et définit la couleur de l'axe horizontal dans le groupe de sparkline.

```csharp
public CellsColor HorizontalAxisColor { get; set; }
```

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(4);

            // Créer un groupe de sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Définir la couleur de l'axe horizontal
            CellsColor axisColor = workbook.CreateCellsColor();
            axisColor.Color = Color.Blue;
            group.HorizontalAxisColor = axisColor;
            group.ShowHorizontalAxis = true;

            // Enregistrez le classeur
            workbook.Save("SparklineHorizontalAxisColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


