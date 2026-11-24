---
title: "TextBoxCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextBoxCollection-Methode. Fügt ein Textfeld zur Sammlung hinzu"
type: docs
url: /de/net/aspose.cells.drawing/textboxcollection/add/
---
## TextBoxCollection.Add method

Fügt der Sammlung ein TextBox hinzu.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| topRow | Int32 | Index der oberen linken Zeile. |
| leftColumn | Int32 | Index der oberen linken Spalte. |
| Höhe | Int32 | Höhe des Textfelds, in Pixel. |
| Breite | Int32 | Breite des Textfelds, in Pixel. |

### Rückgabewert

[`TextBox`](../../textbox/) object index.

### Beispiele

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

### Siehe auch

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


