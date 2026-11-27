---
title: "SparklineGroup.FirstPointColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SparklineGroup-egenskap. Hämtar och anger färgen på den första datapunkten i sparkline-gruppen"
type: docs
url: /sv/net/aspose.cells.charts/sparklinegroup/firstpointcolor/
---
## SparklineGroup.FirstPointColor property

Hämtar och anger färgen på den första datapunkten i sparkline‑gruppen.

```csharp
public CellsColor FirstPointColor { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(4);

            // Skapa sparkline-grupp
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 1;
            ca.EndColumn = 1;
            
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Ange FirstPointColor
            group.ShowFirstPoint = true;
            CellsColor firstPointColor = workbook.CreateCellsColor();
            firstPointColor.Color = Color.Purple;
            group.FirstPointColor = firstPointColor;

            // Spara arbetsboken
            workbook.Save("SparklineFirstPointColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


