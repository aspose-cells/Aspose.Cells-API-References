---
title: "Shape.GetInputRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Gibt den Bereich zurück, der zum Ausfüllen der Steuerung verwendet wird"
type: docs
url: /de/net/aspose.cells.drawing/shape/getinputrange/
---
## Shape.GetInputRange method

Ermittelt den für die Steuerung verwendeten Bereich.

```csharp
public string GetInputRange(bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |

### Rückgabewert

Der Bereich, der zum Ausfüllen der Steuerung verwendet wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetInputRangeWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Input 1");
            worksheet.Cells["A2"].PutValue("Input 2");
            worksheet.Cells["A3"].PutValue("Input 3");

            // Füge eine Listbox-Form hinzu
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 0, 0);
            Shape shape = listBox;

            // Setze den Eingabebereich für die Listbox
            shape.SetInputRange("$A$1:$A$3", false, false);

            // Den Eingabebereich abrufen
            string range = shape.GetInputRange(false, true);
            Console.WriteLine("Shape input range: " + range);
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


