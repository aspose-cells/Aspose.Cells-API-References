---
title: "Cells.SetColumnWidthPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Setzt die Spaltenbreite in Pixeln in der Normalansicht."
type: docs
url: /de/net/aspose.cells/cells/setcolumnwidthpixel/
---
## Cells.SetColumnWidthPixel method

Setzt die Spaltenbreite in Pixeln in der Normalansicht.

```csharp
public void SetColumnWidthPixel(int column, int pixels)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Spaltenindex. |
| Pixel | Int32 | Anzahl der Pixel. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Setze die Spaltenbreiten in Pixeln für die Spalten 1 bis 5
            for (int i = 0; i < 5; i++)
            {
                cells.SetColumnWidthPixel(i, 120); // 120 pixels width
            }

            // Speichere die Arbeitsmappe
            workbook.Save("SetColumnWidthPixelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


