---
title: "Cells.SetViewColumnWidthPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Setzt die Breite der Spalte in verschiedenen Ansichten"
type: docs
url: /de/net/aspose.cells/cells/setviewcolumnwidthpixel/
---
## Cells.SetViewColumnWidthPixel method

Setzt die Breite der Spalte in einer anderen Ansicht.

```csharp
public void SetViewColumnWidthPixel(int column, int pixels)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Der Spaltenindex. |
| Pixel | Int32 | Die Breite in Pixeln. |

### Hinweise

Wenn der aktuelle Ansichtstyp PageLayoutView ist, ist die Spaltenbreite gleich der Druckbreite.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetViewColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Beispieldaten festlegen
            sheet.Cells[0, 0].Value = "Sample Text";

            // Berechne die Pixelbreite (100 Pixel in diesem Beispiel)
            int pixelWidth = 100;

            // Setze die Spaltenbreite in Pixeln
            sheet.Cells.SetViewColumnWidthPixel(0, pixelWidth);

            // Speichere die Arbeitsmappe
            wb.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


