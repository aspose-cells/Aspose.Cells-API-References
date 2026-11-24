---
title: "Klasse DrawObjectEventHandler"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.DrawObjectEventHandler‑Klasse. Schnittstelle zum Abrufen von DrawObject und Bound beim Rendern"
type: docs
url: /de/net/aspose.cells.rendering/drawobjecteventhandler/
---
## DrawObjectEventHandler class

Schnittstelle zum Abrufen von DrawObject und Bound beim Rendern.

```csharp
public abstract class DrawObjectEventHandler
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [Draw](../../aspose.cells.rendering/drawobjecteventhandler/draw/)(DrawObject, float, float, float, float) | Implementiert dieses Interface, um beim Rendern DrawObject und Bound zu erhalten. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassDrawObjectEventHandlerDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(12345);
            worksheet.Shapes.AddRectangle(5, 5, 50, 100, 200, 300); // Added missing parameter

            // PDF-Speicheroptionen mit benutzerdefiniertem Render‑Handler erstellen
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectHandler();

            // Arbeitsmappe als PDF mit Rendering‑Anpassungen speichern
            workbook.Save("DrawObjectEventHandlerDemo.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Demonstration der Handhabung verschiedener Render‑Objekttypen
            switch (drawObject.Type)
            {
                case DrawObjectEnum.Cell:
                    Console.WriteLine($"Rendering cell at ({x}, {y})");
                    break;
                    
                case DrawObjectEnum.Image:
                    Console.WriteLine($"Rendering image at ({x}, {y})");
                    break;
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


