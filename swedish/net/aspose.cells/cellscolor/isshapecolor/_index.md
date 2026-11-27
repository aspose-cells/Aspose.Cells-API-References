---
title: "CellsColor.IsShapeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsColor property. Hämtar och anger färgen som ska tillämpas på cell eller form"
type: docs
url: /sv/net/aspose.cells/cellscolor/isshapecolor/
---
## CellsColor.IsShapeColor property

Hämtar och sätter färgen som ska tillämpas på cell eller form.

```csharp
public bool IsShapeColor { get; set; }
```

### Anmärkningar

Färgens uttryck i cellen och formen är olika. Till exempel: temafärgen med samma nyansvärde kommer inte vara densamma i cellen och i formen.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsColorPropertyIsShapeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en CellsColor-instans och ange IsShapeColor
            CellsColor cellsColor = workbook.CreateCellsColor();
            cellsColor.IsShapeColor = true;
            cellsColor.Color = Color.Green;

            // Applicera färgen på en form
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = cellsColor.Color;  // Use the Color property instead of CellsColor directly

            // Spara arbetsboken
            workbook.Save("CellsColorIsShapeColorDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


