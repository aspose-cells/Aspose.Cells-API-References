---
title: "SparklineGroup.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroup. Indique le type de sparkline du groupe de sparklines"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/type/
---
## SparklineGroup.Type property

Indique le type de sparkline du groupe de sparklines.

```csharp
public SparklineType Type { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Créer un groupe de sparklines de type Colonne
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Column, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Changer le type de sparkline en Ligne
            group.Type = SparklineType.Line;

            // Ajouter un sparkline au groupe
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Enregistrez le classeur
            workbook.Save("SparklineTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


