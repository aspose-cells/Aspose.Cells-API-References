---
title: "SparklineGroup.FirstPointColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroup. Obtient et définit la couleur du premier point de données du groupe de sparklines"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/firstpointcolor/
---
## SparklineGroup.FirstPointColor property

Obtient et définit la couleur du premier point de données dans le groupe de sparkline.

```csharp
public CellsColor FirstPointColor { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyFirstPointColorDemo
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
            ca.StartColumn = 1;
            ca.EndColumn = 1;
            
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Définir FirstPointColor
            group.ShowFirstPoint = true;
            CellsColor firstPointColor = workbook.CreateCellsColor();
            firstPointColor.Color = Color.Purple;
            group.FirstPointColor = firstPointColor;

            // Enregistrez le classeur
            workbook.Save("SparklineFirstPointColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


