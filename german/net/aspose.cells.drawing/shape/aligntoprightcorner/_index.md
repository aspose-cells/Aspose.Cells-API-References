---
title: "Shape.AlignTopRightCorner"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Verschiebt das Bild in die obere rechte Ecke"
type: docs
url: /de/net/aspose.cells.drawing/shape/aligntoprightcorner/
---
## Shape.AlignTopRightCorner method

Verschiebt das Bild in die obere rechte Ecke.

```csharp
public void AlignTopRightCorner(int topRow, int rightColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | der Zeilenindex. |
| rightColumn | Int32 | Der Spaltenindex. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAlignTopRightCornerWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Beispiel shape zum Ausrichten hinzu
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Richte die obere rechte Ecke des shape an Zeile 2, Spalte 5 aus
            shape.AlignTopRightCorner(2, 5);

            // Speichere die Arbeitsmappe
            workbook.Save("AlignTopRightCornerDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


