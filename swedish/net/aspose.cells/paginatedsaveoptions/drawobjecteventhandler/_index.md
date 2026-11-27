---
title: "PaginatedSaveOptions.DrawObjectEventHandler"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions egenskap. Implementerar detta gränssnitt för att hämta DrawObject och Bound vid rendering"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/drawobjecteventhandler/
---
## PaginatedSaveOptions.DrawObjectEventHandler property

Implementerar detta gränssnitt för att hämta DrawObject och Bound vid rendering.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyDrawObjectEventHandlerDemo
    {
        private class CustomDrawObjectEventHandler : DrawObjectEventHandler
        {
            public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
            {
                Console.WriteLine($"DrawObject Type: {drawObject.Type}");
                Console.WriteLine($"Position: X={x}, Y={y}, Width={width}, Height={height}");
            }
        }

        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till lite exempeldata och former
            worksheet.Cells["A1"].PutValue("Test DrawObjectEventHandler");
            worksheet.Cells["A2"].PutValue("This will demonstrate the event handler during rendering");
            
            // Skapa en instans av PaginatedSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Visa det aktuella värdet för egenskapen (bör vara null initialt)
            Console.WriteLine("Current DrawObjectEventHandler value: " + (saveOptions.DrawObjectEventHandler == null ? "null" : "assigned"));
            
            // Ställ in en ny anpassad händelsehanterare
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
            
            // Detta kommer att utlösa Draw-metoden under rendering
            workbook.Save("PropertyDrawObjectEventHandlerDemo.pdf", saveOptions);
            
            // Ändra händelsehanteraren till null för att demonstrera skillnaden
            saveOptions.DrawObjectEventHandler = null;
            workbook.Save("PropertyDrawObjectEventHandlerDemo_NoHandler.pdf", saveOptions);
        }
    }
}
```

### Se även

* class [DrawObjectEventHandler](../../../aspose.cells.rendering/drawobjecteventhandler/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


