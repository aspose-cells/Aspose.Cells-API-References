---
title: "PaginatedSaveOptions.DrawObjectEventHandler"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/drawobjecteventhandler/
---
## PaginatedSaveOptions.DrawObjectEventHandler property

Implementiert dieses Interface, um beim Rendern DrawObject und Bound zu erhalten.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Beispieldaten und Formen hinzufügen
            worksheet.Cells["A1"].PutValue("Test DrawObjectEventHandler");
            worksheet.Cells["A2"].PutValue("This will demonstrate the event handler during rendering");
            
            // Eine Instanz von PaginatedSaveOptions erstellen
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Den aktuellen Wert der Eigenschaft anzeigen (sollte zunächst null sein)
            Console.WriteLine("Current DrawObjectEventHandler value: " + (saveOptions.DrawObjectEventHandler == null ? "null" : "assigned"));
            
            // Einen neuen benutzerdefinierten Ereignishandler festlegen
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
            
            // Dies löst die Draw‑Methode beim Rendern aus
            workbook.Save("PropertyDrawObjectEventHandlerDemo.pdf", saveOptions);
            
            // Den Ereignishandler auf null setzen, um den Unterschied zu demonstrieren
            saveOptions.DrawObjectEventHandler = null;
            workbook.Save("PropertyDrawObjectEventHandlerDemo_NoHandler.pdf", saveOptions);
        }
    }
}
```

### Siehe auch

* class [DrawObjectEventHandler](../../../aspose.cells.rendering/drawobjecteventhandler/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


