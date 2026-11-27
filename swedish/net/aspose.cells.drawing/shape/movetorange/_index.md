---
title: "Shape.MoveToRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape‑metod. Flyttar formen till ett angivet område"
type: docs
url: /sv/net/aspose.cells.drawing/shape/movetorange/
---
## Shape.MoveToRange method

Flyttar formen till ett angivet område.

```csharp
public void MoveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| bottomRow | Int32 | Index för nedre högra rad |
| rightColumn | Int32 | Index för nedre högra kolumnen |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodMoveToRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Flytta formen till ett specifikt område
            shape.MoveToRange(12, 3, 13, 5);

            // Spara arbetsboken
            workbook.Save("ShapeMoveToRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


