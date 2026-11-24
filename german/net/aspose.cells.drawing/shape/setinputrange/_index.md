---
title: "Shape.SetInputRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Methode. Legt den Bereich fest, der zum Befüllen des Steuerelements verwendet wird"
type: docs
url: /de/net/aspose.cells.drawing/shape/setinputrange/
---
## Shape.SetInputRange method

Legt den für die Steuerung verwendeten Bereich fest.

```csharp
public void SetInputRange(string formula, bool isR1C1, bool isLocal)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Formel | String | Der Bereich, der zum Ausfüllen der Steuerung verwendet wird. |
| isR1C1 | Boolean | Ob die Formel im R1C1-Format formatiert werden muss. |
| isLocal | Boolean | Ob die Formel nach den Ländereinstellungen formatiert werden muss. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetInputRangeWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Ein Arbeitsmappenobjekt erstellen
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu den Zellen A1:A10 hinzu
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Füge eine Listbox-Form hinzu
            Aspose.Cells.Drawing.Shape listBox = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);

            // Setze den Eingabebereich für die Listbox (unter Verwendung von String-, Boolean- und Boolean-Parametern)
            listBox.SetInputRange("$A$1:$A$6", false, false);

            // Setze die verknüpfte Zelle für die Listbox
            listBox.SetLinkedCell("$A$12", false, true);

            // Speichere die Arbeitsmappe
            workbook.Save("SetInputRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


