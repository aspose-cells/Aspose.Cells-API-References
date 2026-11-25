---
title: "Class DrawObjectEventHandler"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.DrawObjectEventHandler. Interfaccia per ottenere DrawObject e Bound durante il rendering"
type: docs
url: /it/net/aspose.cells.rendering/drawobjecteventhandler/
---
## DrawObjectEventHandler class

Interfaccia per ottenere DrawObject e Bound durante il rendering.

```csharp
public abstract class DrawObjectEventHandler
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [Draw](../../aspose.cells.rendering/drawobjecteventhandler/draw/)(DrawObject, float, float, float, float) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |

### Esempi

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
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(12345);
            worksheet.Shapes.AddRectangle(5, 5, 50, 100, 200, 300); // Added missing parameter

            // Crea opzioni di salvataggio PDF con gestore di rendering personalizzato
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectHandler();

            // Salva la cartella di lavoro in PDF con personalizzazione del rendering
            workbook.Save("DrawObjectEventHandlerDemo.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Dimostra la gestione di diversi tipi di oggetti di rendering
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

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


