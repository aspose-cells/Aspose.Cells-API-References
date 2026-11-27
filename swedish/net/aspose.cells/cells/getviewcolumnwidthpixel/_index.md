---
title: "Cells.GetViewColumnWidthPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämta bredden i olika vystyper"
type: docs
url: /sv/net/aspose.cells/cells/getviewcolumnwidthpixel/
---
## Cells.GetViewColumnWidthPixel method

Hämta bredden i olika vystyper.

```csharp
public int GetViewColumnWidthPixel(int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| column | Int32 | Kolumnindexet. |

### Returvärde

kolumnbredden i enheten pixlar

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in vystyper till PageLayoutView
            worksheet.ViewType = ViewType.PageLayoutView;
            
            // Ställ in kolumnbredd i tecken (kommer att konverteras till pixlar)
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Hämta kolumnbredden i pixlar
            int columnWidthInPixels = worksheet.Cells.GetViewColumnWidthPixel(0);
            
            // Skriv ut resultatet
            Console.WriteLine("Column width in pixels: " + columnWidthInPixels);
            
            // Spara arbetsboken
            workbook.Save("ColumnWidthTest.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


