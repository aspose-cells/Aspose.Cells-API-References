---
title: "Shape.GetLinkedCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape Methode. Gibt den Bereich zurück, der mit dem Wert des Steuerelements verknüpft ist."
type: docs
url: /de/net/aspose.cells.drawing/shape/getlinkedcell/
---
## Shape.GetLinkedCell method

Ermittelt den mit dem Wert der Steuerung verknüpften Bereich.

```csharp
public string GetLinkedCell(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |

### Rückgabewert

Der Bereich, der mit dem Wert des Steuerelements verknüpft ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetLinkedCellWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Form hinzufügen und deren verknüpfte Zelle festlegen
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.LinkedCell = "A1";

            // Die Adresse der verknüpften Zelle mit verschiedenen Parameterkombinationen abrufen
            string link1 = shape.GetLinkedCell(false, false); // Returns absolute reference like "$A$1"
            string link2 = shape.GetLinkedCell(true, false);   // Returns relative reference like "A1"
            string link3 = shape.GetLinkedCell(false, true);   // Returns R1C1 style absolute reference

            Console.WriteLine("Linked cell (absolute A1): " + link1);
            Console.WriteLine("Linked cell (relative A1): " + link2);
            Console.WriteLine("Linked cell (R1C1 style): " + link3);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


