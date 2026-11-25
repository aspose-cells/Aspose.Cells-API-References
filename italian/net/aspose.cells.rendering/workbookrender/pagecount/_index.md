---
title: "WorkbookRender.PageCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookRender. Ottiene il conteggio totale delle pagine della cartella di lavoro"
type: docs
url: /it/net/aspose.cells.rendering/workbookrender/pagecount/
---
## WorkbookRender.PageCount property

Ottiene il conteggio totale delle pagine della cartella di lavoro.

```csharp
public int PageCount { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderPropertyPageCountDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // Aggiungi un secondo foglio di lavoro
            workbook.Worksheets.Add();
            worksheet = workbook.Worksheets[1];
            worksheet.Cells["A1"].PutValue("Page 2 Content");

            // Crea opzioni di rendering e il renderer della cartella di lavoro
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };
            
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Dimostra l'uso di PageCount
            Console.WriteLine($"Total pages to render: {renderer.PageCount}");
            
            // Renderizza ogni pagina in immagine
            for (int i = 0; i < renderer.PageCount; i++)
            {
                string outputPath = $"Page_{i}.png";
                renderer.ToImage(i, outputPath);
                Console.WriteLine($"Rendered page {i+1} to {outputPath}");
            }
        }
    }
}
```

### Vedi anche

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


