---
title: "SparklineGroup.ShowLastPoint"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Indica se evidenziare l'ultimo punto dei dati nel gruppo sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/showlastpoint/
---
## SparklineGroup.ShowLastPoint property

Indica se evidenziare l'ultimo punto dati nel gruppo di sparkline.

```csharp
public bool ShowLastPoint { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowLastPointDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Crea gruppo sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Aggiungi sparkline
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Configura l'aspetto dello sparkline
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;
            group.LineWeight = 1.0;

            // Abilita e colora l'ultimo punto
            group.ShowLastPoint = true;
            CellsColor lastPointColor = workbook.CreateCellsColor();
            lastPointColor.Color = Color.Yellow;
            group.LastPointColor = lastPointColor;

            // Salva la cartella di lavoro
            workbook.Save("SparklineShowLastPointDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


