---
title: "SheetSet.Visible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SheetSet. Restituisce un insieme con i fogli visibili del workbook nel loro ordine originale"
type: docs
url: /it/net/aspose.cells.rendering/sheetset/visible/
---
## SheetSet.Visible property

Ottiene un insieme con i fogli visibili della cartella di lavoro nel loro ordine originale.

```csharp
public static SheetSet Visible { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyVisibleDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con due fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Nascondi il secondo foglio di lavoro
            workbook.Worksheets[1].IsVisible = false;

            // Imposta le opzioni di salvataggio per esportare solo i fogli visibili
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                SheetSet = SheetSet.Visible
            };

            // Salva il workbook (verrà esportato solo il foglio visibile)
            workbook.Save("VisibleSheetsOnly.pptx", saveOptions);

            Console.WriteLine("Workbook saved with only visible sheets exported.");
        }
    }
}
```

### Vedi anche

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


