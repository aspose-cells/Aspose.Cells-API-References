---
title: "Shape.LinkedCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den mit dem Steuerelementwert verknüpften Arbeitsblattbereich zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/shape/linkedcell/
---
## Shape.LinkedCell property

Liest oder setzt den Arbeitsblattbereich, der mit dem Wert des Steuerelements verknüpft ist.

```csharp
public string LinkedCell { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt eine Form hinzu
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Setzen Sie die LinkedCell-Eigenschaft auf B6
            shape.LinkedCell = "$B$6";

            // Ändern Sie die LinkedCell zu A1, wenn sie B6 war
            if (shape.LinkedCell.Equals("$B$6"))
            {
                shape.LinkedCell = "A1";
            }

            // Geben Sie den aktuellen LinkedCell-Wert aus
            Console.WriteLine("Shape's LinkedCell: " + shape.LinkedCell);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


