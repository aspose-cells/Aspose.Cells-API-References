---
title: "WorkbookRender.WorkbookRender"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore WorkbookRender. La costruzione di WorkbookRender"
type: docs
url: /it/net/aspose.cells.rendering/workbookrender/workbookrender/
---
## WorkbookRender constructor

La costruzione di WorkbookRender

```csharp
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cartella di lavoro | Cartella di lavoro | Indica quale cartella di lavoro deve essere renderizzata. |
| opzioni | ImageOrPrintOptions | ImageOrPrintOptions contiene alcune proprietà dell'immagine di output |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodctorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Crea opzioni di immagine/stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Crea il renderer della cartella di lavoro
            WorkbookRender renderer = new WorkbookRender(workbook, options);
            
            // Conteggio delle pagine di output
            Console.WriteLine("Total pages: " + renderer.PageCount);
        }
    }
}
```

### Vedi anche

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


