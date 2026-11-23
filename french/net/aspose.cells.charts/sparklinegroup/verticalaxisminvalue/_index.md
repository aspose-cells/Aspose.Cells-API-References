---
title: "SparklineGroup.VerticalAxisMinValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroup. Obtient et définit la valeur minimale personnalisée pour l'axe vertical."
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/verticalaxisminvalue/
---
## SparklineGroup.VerticalAxisMinValue property

Obtient et définit la valeur minimale personnalisée pour l'axe vertical.

```csharp
public double VerticalAxisMinValue { get; set; }
```

### Remarques

Si cette propriété est définie, [`VerticalAxisMinValueType`](../verticalaxisminvaluetype/) sera Custom.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMinValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(2);
            sheet.Cells["A3"].PutValue(1);
            sheet.Cells["A4"].PutValue(3);

            // Créer un groupe de sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Définir la valeur minimale de l'axe vertical
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMinValue = 0.0;

            // Enregistrez le classeur
            workbook.Save("SparklineVerticalAxisMinValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


