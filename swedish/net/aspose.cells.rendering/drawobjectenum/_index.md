---
title: "Enum DrawObjectEnum"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Rendering.DrawObjectEnum enum. Anger Cell eller Image för DrawObject"
type: docs
url: /sv/net/aspose.cells.rendering/drawobjectenum/
---
## DrawObjectEnum enumeration

Indikera cell eller bild för DrawObject.

```csharp
public enum DrawObjectEnum
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Image | `0` | Anger att DrawObject är en Image |
| Cell | `1` | anger att DrawObject är en Cell |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassDrawObjectEnumDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Cell");

            // Skapa ett PdfSaveOptions-objekt
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Skapa en anpassad DrawObjectEventHandler
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Spara arbetsboken som PDF med den anpassade hanteraren
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Kontrollera om ritobjektet är en cell
            if (drawObject.Type == DrawObjectEnum.Cell)
            {
                Cell cell = drawObject.Cell;
                
                // Skriv ut cellinformation
                Console.WriteLine($"Drawing Cell - Row: {cell.Row}, Column: {cell.Column}");
                Console.WriteLine($"Position: ({x}, {y}), Size: {width}x{height}");
                
                // Speciell hantering för cell A1
                if (cell.Row == 0 && cell.Column == 0)
                {
                    Console.WriteLine("This is cell A1");
                }
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


