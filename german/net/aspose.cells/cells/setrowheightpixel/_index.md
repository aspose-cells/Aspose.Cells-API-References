---
title: "Cells.SetRowHeightPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Setzt die Zeilenhöhe in Pixel"
type: docs
url: /de/net/aspose.cells/cells/setrowheightpixel/
---
## Cells.SetRowHeightPixel method

Setzt die Zeilenhöhe in Pixeln.

```csharp
public void SetRowHeightPixel(int row, int pixels)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |
| Pixel | Int32 | Anzahl der Pixel. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Setze die Höhe der ersten Zeile auf 50 Pixel
            worksheet.Cells.SetRowHeightPixel(0, 50);

            // Setze die Höhe der zweiten Zeile auf 100 Pixel
            worksheet.Cells.SetRowHeightPixel(1, 100);

            // Speichere die Arbeitsmappe
            workbook.Save("RowHeightPixelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


