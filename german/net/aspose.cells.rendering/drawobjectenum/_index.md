---
title: "Enum DrawObjectEnum"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.DrawObjectEnum‑Enum. Gibt an, ob das DrawObject eine Zelle oder ein Bild ist"
type: docs
url: /de/net/aspose.cells.rendering/drawobjectenum/
---
## DrawObjectEnum enumeration

Kennzeichnet Zelle oder Bild des DrawObject.

```csharp
public enum DrawObjectEnum
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Image | `0` | Gibt an, dass DrawObject ein Bild ist |
| Cell | `1` | Gibt an, dass DrawObject eine Zelle ist |

### Beispiele

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
            // Erstelle eine Arbeitsmappe und füge Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Cell");

            // Erstelle ein PdfSaveOptions-Objekt
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Erstelle einen benutzerdefinierten DrawObjectEventHandler
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Speichern Sie die Arbeitsmappe als PDF mit dem benutzerdefinierten Handler
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Prüfen, ob das Zeichenobjekt eine Zelle ist
            if (drawObject.Type == DrawObjectEnum.Cell)
            {
                Cell cell = drawObject.Cell;
                
                // Zellinformationen ausgeben
                Console.WriteLine($"Drawing Cell - Row: {cell.Row}, Column: {cell.Column}");
                Console.WriteLine($"Position: ({x}, {y}), Size: {width}x{height}");
                
                // Spezielle Behandlung für Zelle A1
                if (cell.Row == 0 && cell.Column == 0)
                {
                    Console.WriteLine("This is cell A1");
                }
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


