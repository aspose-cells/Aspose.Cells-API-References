---
title: "SparklineGroup.VerticalAxisMaxValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroup. Obtient et définit la valeur maximale personnalisée pour l'axe vertical"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/verticalaxismaxvalue/
---
## SparklineGroup.VerticalAxisMaxValue property

Obtient et définit la valeur maximale personnalisée pour l'axe vertical.

```csharp
public double VerticalAxisMaxValue { get; set; }
```

### Remarques

Si cette propriété est définie, [`VerticalAxisMaxValueType`](../verticalaxismaxvaluetype/) sera Custom.

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMaxValueDemo
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

            // Définir l'emplacement du sparkline
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

            // Ajouter un sparkline
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Définir la valeur maximale de l'axe vertical
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMaxValue = 10.0;

            // Enregistrez le classeur
            workbook.Save("SparklineVerticalAxisMaxValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


