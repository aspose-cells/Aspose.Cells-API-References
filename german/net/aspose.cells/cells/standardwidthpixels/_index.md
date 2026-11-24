---
title: "Cells.StandardWidthPixels"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt die Standardspaltenbreite im Arbeitsblatt in Pixeln zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/cells/standardwidthpixels/
---
## Cells.StandardWidthPixels property

Liest oder setzt die Standardspaltenbreite im Arbeitsblatt, in Pixel.

```csharp
public int StandardWidthPixels { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthPixelsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setze und lese die Standardbreite in Pixeln
            cells.StandardWidthPixels = 104;
            Console.WriteLine("Standard Width in Pixels: " + cells.StandardWidthPixels);

            // Setze und lese die Standardbreite in Zeichen
            cells.StandardWidth = 12.375;
            Console.WriteLine("Standard Width in Characters: " + cells.StandardWidth);

            // Setze und lese die Standardhöhe in Punkten
            cells.StandardHeight = 14.25;
            Console.WriteLine("Standard Height in Points: " + cells.StandardHeight);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


