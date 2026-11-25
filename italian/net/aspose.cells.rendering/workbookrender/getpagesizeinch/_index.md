---
title: "WorkbookRender.GetPageSizeInch"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorkbookRender. Ottiene la dimensione della pagina in pollici dell'immagine di output"
type: docs
url: /it/net/aspose.cells.rendering/workbookrender/getpagesizeinch/
---
## WorkbookRender.GetPageSizeInch method

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

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodGetPageSizeInchWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Test page size");
            sheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            WorkbookRender wr = new WorkbookRender(wb, imgOpt);
            
            float[] pageSize = wr.GetPageSizeInch(0);
            Console.WriteLine($"Page size in inches: {pageSize[0]} x {pageSize[1]}");
        }
    }
}
```

### Vedi anche

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


