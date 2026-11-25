---
title: "SheetRender.GetPageSizeInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SheetRender. Ottieni la dimensione della pagina in pollici dell'immagine di output"
type: docs
url: /it/net/aspose.cells.rendering/sheetrender/getpagesizeinch/
---
## SheetRender.GetPageSizeInch method

Ottieni la dimensione della pagina in pollici dell'immagine di output.

```csharp
public float[] GetPageSizeInch(int pageIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | L'indice della pagina è basato su zero. |

### Valore di ritorno

Dimensione dell'immagine, [0] per la larghezza e [1] per l'altezza

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.PageSetup.PrintArea = "A1:D10";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true,
                ImageType = ImageType.Png
            };

            SheetRender sheetRender = new SheetRender(worksheet, options);
            float[] pageSize = sheetRender.GetPageSizeInch(0);
            
            Console.WriteLine($"Page Size (Inches): Width={pageSize[0]}, Height={pageSize[1]}");
        }
    }
}
```

### Vedi anche

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


