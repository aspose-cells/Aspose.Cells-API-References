---
title: "SparklineGroup.SeriesColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SparklineGroup. Obtient et définit la couleur des sparklines dans le groupe de sparklines"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroup/seriescolor/
---
## SparklineGroup.SeriesColor property

Obtient et définit la couleur des sparklines dans le groupe de sparkline.

```csharp
public CellsColor SeriesColor { get; set; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertySeriesColorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Données d'exemple
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(8);
            ws.Cells["A3"].PutValue(3);
            
            // Créer un groupe de sparkline
            CellArea dataRange = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            CellArea locationRange = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 1, EndColumn = 1 };
            int index = ws.SparklineGroups.Add(SparklineType.Column, "A1:A3", false, locationRange);
            
            // Définir la couleur de la série
            SparklineGroup group = ws.SparklineGroups[index];
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;
            
            wb.Save("SparklineSeriesColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


