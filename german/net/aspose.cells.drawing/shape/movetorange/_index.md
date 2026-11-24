---
title: "Shape.MoveToRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Verschiebt das Shape in einen angegebenen Bereich"
type: docs
url: /de/net/aspose.cells.drawing/shape/movetorange/
---
## Shape.MoveToRange method

Verschiebt die Form in einen angegebenen Bereich.

```csharp
public void MoveToRange(int topRow, int leftColumn, int bottomRow, int rightColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| bottomRow | Int32 | Index der unteren rechten Zeile |
| rightColumn | Int32 | Index der unteren rechten Spalte |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Verschieben Sie das Shape in einen bestimmten Bereich
            shape.MoveToRange(12, 3, 13, 5);

            // Speichere die Arbeitsmappe
            workbook.Save("ShapeMoveToRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


