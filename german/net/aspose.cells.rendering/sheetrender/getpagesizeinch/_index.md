---
title: "SheetRender.GetPageSizeInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SheetRender-Methode. Ermittelt die Seitengröße in Zoll des Ausgabebildes"
type: docs
url: /de/net/aspose.cells.rendering/sheetrender/getpagesizeinch/
---
## SheetRender.GetPageSizeInch method

Ermittelt die Seitengröße in Zoll des Ausgabebildes.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seitenindex | Int32 | Der Seitenindex basiert auf Null. |

### Rückgabewert

Bildgröße, [0] für Breite und [1] für Höhe

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.PrintArea = "A1:D10";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true,
                ImageType = ImageType.Png
            };

            SheetRender sheetRender = new SheetRender(worksheet, options);
            float[] pageSize = sheetRender.GetPageSizeInch(0);
            
            Console.WriteLine($"Page Size (Inches): Width={pageSize[0]}, Height={pageSize[1]}");
        }
    }
}
```

### Siehe auch

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


