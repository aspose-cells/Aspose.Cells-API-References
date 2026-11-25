---
title: "PaginatedSaveOptions.DrawObjectEventHandler"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/drawobjecteventhandler/
---
## PaginatedSaveOptions.DrawObjectEventHandler property

Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati di esempio e forme
            worksheet.Cells["A1"].PutValue("Test DrawObjectEventHandler");
            worksheet.Cells["A2"].PutValue("This will demonstrate the event handler during rendering");
            
            // Crea un'istanza di PaginatedSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Visualizza il valore corrente della proprietà (dovrebbe essere null inizialmente)
            Console.WriteLine("Current DrawObjectEventHandler value: " + (saveOptions.DrawObjectEventHandler == null ? "null" : "assigned"));
            
            // Imposta un nuovo gestore di eventi personalizzato
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();
            
            // Questo attiverà il metodo Draw durante il rendering
            workbook.Save("PropertyDrawObjectEventHandlerDemo.pdf", saveOptions);
            
            // Cambia il gestore di eventi a null per dimostrare la differenza
            saveOptions.DrawObjectEventHandler = null;
            workbook.Save("PropertyDrawObjectEventHandlerDemo_NoHandler.pdf", saveOptions);
        }
    }
}
```

### Vedi anche

* class [DrawObjectEventHandler](../../../aspose.cells.rendering/drawobjecteventhandler/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


