---
title: "SparklineGroup.Sparklines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Ottiene la raccolta di oggetti Sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/sparklines/
---
## SparklineGroup.Sparklines property

Ottiene la raccolta di oggetto [`Sparkline`](../../sparkline/).

```csharp
public SparklineCollection Sparklines { get; }
```

### Esempi

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

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Crea gruppo sparkline
            CellArea location = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 4, EndColumn = 4 };
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Aggiungi sparkline usando la proprietà Sparklines
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Personalizza l'aspetto della sparkline
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;

            // Salva la cartella di lavoro
            workbook.Save("SparklineDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


