---
title: "Cells.GetViewColumnWidthPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Erhalte die Breite in verschiedenen Ansichtstypen"
type: docs
url: /de/net/aspose.cells/cells/getviewcolumnwidthpixel/
---
## Cells.GetViewColumnWidthPixel method

Erhalte die Breite in verschiedenen Ansichtstypen.

```csharp
public int GetViewColumnWidthPixel(int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| column | Int32 | Der Spaltenindex. |

### Rückgabewert

die Spaltenbreite in Pixeln

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze den Ansichtstyp auf PageLayoutView
            worksheet.ViewType = ViewType.PageLayoutView;
            
            // Spaltenbreite in Zeichen festlegen (wird in Pixel umgerechnet)
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Erhalte die Spaltenbreite in Pixeln
            int columnWidthInPixels = worksheet.Cells.GetViewColumnWidthPixel(0);
            
            // Gib das Ergebnis aus
            Console.WriteLine("Column width in pixels: " + columnWidthInPixels);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ColumnWidthTest.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


