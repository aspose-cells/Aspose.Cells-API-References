---
title: "Klasse PageStartSavingArgs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.PageStartSavingArgs class. Informationen zum Start des Speichervorgangs einer Seite"
type: docs
url: /de/net/aspose.cells.rendering/pagestartsavingargs/
---
## PageStartSavingArgs class

Info für den Beginn des Seiten‑Speichervorgangs.

```csharp
public class PageStartSavingArgs : PageSavingArgs
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IsToOutput](../../aspose.cells.rendering/pagestartsavingargs/istooutput/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob die Seite ausgegeben werden soll. Der Standardwert ist true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Gesamtseitenzahl.(Vererbt von [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Aktueller Seitenindex, nullbasiert.(Vererbt von [`PageSavingArgs`](../pagesavingargs/).) |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageStartSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Hello World");
            
            PdfSaveOptions options = new PdfSaveOptions();
            options.PageSavingCallback = new CustomPageSavingCallback();
            
            workbook.Save("output.pdf", options);
        }
    }
    
    public class CustomPageSavingCallback : IPageSavingCallback
    {
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }
        
        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Optionale Implementierung
        }
    }
}
```

### Siehe auch

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


