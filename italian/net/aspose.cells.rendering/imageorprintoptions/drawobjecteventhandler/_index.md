---
title: "ImageOrPrintOptions.DrawObjectEventHandler"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/
---
## ImageOrPrintOptions.DrawObjectEventHandler property

Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDrawObjectEventHandlerDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);

            // Crea un gestore di eventi DrawObject personalizzato
            var drawHandler = new CustomDrawObjectEventHandler();

            // Imposta le opzioni immagine con il gestore dell'evento
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.DrawObjectEventHandler = drawHandler;

            // Esegui il rendering del foglio di lavoro per attivare gli eventi
            SheetRender render = new SheetRender(worksheet, options);
            for (int pageIndex = 0; pageIndex < render.PageCount; pageIndex++)
            {
                using (MemoryStream stream = new MemoryStream())
                {
                    render.ToImage(pageIndex, stream);
                }
            }
        }
    }

    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Esempio: Stampa le informazioni sull'oggetto disegnato
            Console.WriteLine($"Drawing {drawObject.Type} at ({x},{y}) with size {width}x{height}");
        }
    }
}
```

### Vedi anche

* class [DrawObjectEventHandler](../../drawobjecteventhandler/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


