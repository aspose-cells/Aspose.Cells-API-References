---
title: "TextBoxCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextBoxCollection-metod. Lägger till en textruta i samlingen"
type: docs
url: /sv/net/aspose.cells.drawing/textboxcollection/add/
---
## TextBoxCollection.Add method

Lägger till en textruta i samlingen.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| höjd | Int32 | Höjd på textbox, i enhet pixel. |
| bredd | Int32 | Bredd på textbox, i enhet pixel. |

### Returvärde

[`TextBox`](../../textbox/) object index.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int index = worksheet.TextBoxes.Add(1, 1, 50, 100);
            Console.WriteLine("TextBox added at index: " + index);
        }
    }
}
```

### Se även

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


