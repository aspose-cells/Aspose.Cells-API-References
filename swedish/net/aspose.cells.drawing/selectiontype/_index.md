---
title: "Enum SelectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.SelectionType enum. Urvalstypen för listboxen"
type: docs
url: /sv/net/aspose.cells.drawing/selectiontype/
---
## SelectionType enumeration

Urvalstypen för listboxen.

```csharp
public enum SelectionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Single | `0` | Enkel urvalstyp. |
| Multi | `1` | Multipel urvalstyp. |
| Extend | `2` | Utökad urvalstyp. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassSelectionTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en listbox i kalkylbladet
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 5, 10);

            // Ställ in urvalstypen till Enkel
            listBox.SelectionType = SelectionType.Single;

            // Lägg till objekt i listboxen
            listBox.SetInputRange("A1:A5", false, false);

            // Verifiera urvalstypen
            Console.WriteLine("ListBox SelectionType: " + listBox.SelectionType);

            // Spara arbetsboken
            workbook.Save("SelectionTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


