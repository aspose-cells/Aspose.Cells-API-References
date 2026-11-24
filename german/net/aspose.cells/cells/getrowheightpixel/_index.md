---
title: "Cells.GetRowHeightPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells‑Methode. Gibt die Höhe einer angegebenen Zeile in Pixel zurück."
type: docs
url: /de/net/aspose.cells/cells/getrowheightpixel/
---
## Cells.GetRowHeightPixel method

Gibt die Höhe einer angegebenen Zeile in Pixel zurück.

```csharp
public int GetRowHeightPixel(int row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex |

### Rückgabewert

Höhe der Zeile

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightPixelWithInt32Demo
    {
        public static void Run()
        {
            // Instanziieren Sie ein neues Arbeitsbuch
            Workbook wb = new Workbook();

            // Hole das erste Arbeitsblatt
            Worksheet worksheet = wb.Worksheets[0];

            // Zeilenhöhe für Zeile 5 festlegen (in Pixeln)
            worksheet.Cells.SetRowHeightPixel(5, 30);

            // Zeilenhöhe für Zeile 5 abrufen (in Pixeln)
            int rowHeight = worksheet.Cells.GetRowHeightPixel(5);

            Console.WriteLine("Row height of row 5 in pixels: " + rowHeight);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


