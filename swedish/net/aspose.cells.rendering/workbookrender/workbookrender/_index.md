---
title: "WorkbookRender.WorkbookRender"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookRender-konstruktor. Konstruktionen av WorkbookRender"
type: docs
url: /sv/net/aspose.cells.rendering/workbookrender/workbookrender/
---
## WorkbookRender constructor

Konstruktionen av WorkbookRender

```csharp
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arbetsbok | Arbetsbok | Ange vilken arbetsbok som ska renderas. |
| alternativ | ImageOrPrintOptions | ImageOrPrintOptions innehåller vissa egenskaper för utdatabild |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodctorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Skapa bild-/utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Skapa arbetsboksgenererare
            WorkbookRender renderer = new WorkbookRender(workbook, options);
            
            // Utdata sidantal
            Console.WriteLine("Total pages: " + renderer.PageCount);
        }
    }
}
```

### Se även

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


