---
title: "SparklineGroup.PresetStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroup. Obtient et définit le type de style prédéfini du groupe de sparklines"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/presetstyle/
---
## SparklineGroup.PresetStyle property

Obtient et définit le type de style prédéfini du groupe de sparkline.

```csharp
public SparklinePresetStyleType PresetStyle { get; set; }
```

### Remarques

Si cette propriété est définie, ces propriétés : SeriesColor, NegativePointsColor, HorizontalAxisColor, MarkersColor, FirstPointColor, LastPointColor, HighPointColor, LowPointColor seront couvertes. Veuillez donc définir d'abord la propriété, puis les autres.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPresetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["C1"].PutValue(7);
            worksheet.Cells["D1"].PutValue(2);
            worksheet.Cells["E1"].PutValue(9);

            // Créer un groupe de sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 5;
            ca.EndColumn = 5;
            int index = worksheet.SparklineGroups.Add(SparklineType.Column, "A1:E1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[index];

            // Appliquer le style prédéfini
            group.PresetStyle = SparklinePresetStyleType.Style5;

            workbook.Save("SparklinePresetStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [SparklinePresetStyleType](../../sparklinepresetstyletype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


