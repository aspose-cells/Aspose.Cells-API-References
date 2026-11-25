---
title: "SheetSet.All"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SheetSet. Restituisce un insieme con tutti i fogli del workbook nel loro ordine originale"
type: docs
url: /it/net/aspose.cells.rendering/sheetset/all/
---
## SheetSet.All property

Ottiene un insieme con tutti i fogli della cartella di lavoro nel loro ordine originale.

```csharp
public static SheetSet All { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyAllDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con due fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Imposta alcuni dati di esempio in entrambi i fogli
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Salva tutti i fogli in markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.SheetSet = SheetSet.All;
            
            workbook.Save("output.md", saveOptions);
            Console.WriteLine("All sheets saved to markdown successfully.");
        }
    }
}
```

### Vedi anche

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


