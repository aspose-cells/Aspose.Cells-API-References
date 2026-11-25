---
title: "Enum DrawObjectEnum"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Rendering.DrawObjectEnum. Indica Cell o Image di DrawObject"
type: docs
url: /it/net/aspose.cells.rendering/drawobjectenum/
---
## DrawObjectEnum enumeration

Indica la cella o l'immagine di DrawObject.

```csharp
public enum DrawObjectEnum
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Image | `0` | Indica che DrawObject è un Image |
| Cell | `1` | indica che DrawObject è un Cell |

### Esempi

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
            // Crea una cartella di lavoro e aggiungi dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Cell");

            // Crea un oggetto PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Crea un DrawObjectEventHandler personalizzato
            saveOptions.DrawObjectEventHandler = new CustomDrawObjectEventHandler();

            // Salva la cartella di lavoro in PDF con il gestore personalizzato
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class CustomDrawObjectEventHandler : DrawObjectEventHandler
    {
        public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
        {
            // Verifica se il draw object è una cella
            if (drawObject.Type == DrawObjectEnum.Cell)
            {
                Cell cell = drawObject.Cell;
                
                // Output delle informazioni sulla cella
                Console.WriteLine($"Drawing Cell - Row: {cell.Row}, Column: {cell.Column}");
                Console.WriteLine($"Position: ({x}, {y}), Size: {width}x{height}");
                
                // Gestione speciale per la cella A1
                if (cell.Row == 0 && cell.Column == 0)
                {
                    Console.WriteLine("This is cell A1");
                }
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


