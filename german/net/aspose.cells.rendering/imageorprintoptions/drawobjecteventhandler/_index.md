---
title: "ImageOrPrintOptions.DrawObjectEventHandler"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions Eigenschaft. Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/
---
## ImageOrPrintOptions.DrawObjectEventHandler property

Implementiert dieses Interface, um beim Rendern DrawObject und Bound zu erhalten.

```csharp
public DrawObjectEventHandler DrawObjectEventHandler { get; set; }
```

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);

            // Erstelle benutzerdefinierten DrawObject-Ereignishandler
            var drawHandler = new CustomDrawObjectEventHandler();

            // Setze Bildoptionen mit dem Ereignishandler
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.DrawObjectEventHandler = drawHandler;

            // Render das Arbeitsblatt, um die Ereignisse auszulösen
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
            // Beispiel: Informationen über das gezeichnete Objekt ausgeben
            Console.WriteLine($"Drawing {drawObject.Type} at ({x},{y}) with size {width}x{height}");
        }
    }
}
```

### Siehe auch

* class [DrawObjectEventHandler](../../drawobjecteventhandler/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


