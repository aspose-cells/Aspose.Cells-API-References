---
title: "WorkbookRender.GetPageSizeInch"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookRender-Methode. Gibt die Seitengröße in Zoll des Ausgabebildes zurück"
type: docs
url: /de/net/aspose.cells.rendering/workbookrender/getpagesizeinch/
---
## WorkbookRender.GetPageSizeInch method

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

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test page size");
            sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            WorkbookRender wr = new WorkbookRender(wb, imgOpt);
            
            float[] pageSize = wr.GetPageSizeInch(0);
            Console.WriteLine($"Page size in inches: {pageSize[0]} x {pageSize[1]}");
        }
    }
}
```

### Siehe auch

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


