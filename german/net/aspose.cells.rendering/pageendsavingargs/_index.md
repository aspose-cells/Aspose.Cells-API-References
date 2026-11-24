---
title: "Klasse PageEndSavingArgs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.PageEndSavingArgs class. Informationen zum Abschluss des Speichervorgangs einer Seite"
type: docs
url: /de/net/aspose.cells.rendering/pageendsavingargs/
---
## PageEndSavingArgs class

Informationen für eine Seite beenden den Speichervorgang.

```csharp
public class PageEndSavingArgs : PageSavingArgs
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [HasMorePages](../../aspose.cells.rendering/pageendsavingargs/hasmorepages/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob weitere Seiten ausgegeben werden sollen. Der Standardwert ist true. |
| [PageCount](../../aspose.cells.rendering/pagesavingargs/pagecount/) { get; } | Gesamtseitenzahl.(Vererbt von [`PageSavingArgs`](../pagesavingargs/).) |
| [PageIndex](../../aspose.cells.rendering/pagesavingargs/pageindex/) { get; } | Aktueller Seitenindex, nullbasiert.(Vererbt von [`PageSavingArgs`](../pagesavingargs/).) |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassPageEndSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Erstellen Sie eine Instanz von PdfSaveOptions
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Setze den PageEndSaving-Callback
            saveOptions.PageSavingCallback = new PageEndSavingArgsTest();

            // Speichere die Arbeitsmappe mit dem Callback
            workbook.Save("output.pdf", saveOptions);
        }
    }

    public class PageEndSavingArgsTest : IPageSavingCallback
    {
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }

        public void PageStartSaving(PageStartSavingArgs args)
        {
            // Implementierung für diese Demo nicht erforderlich
        }
    }
}
```

### Siehe auch

* class [PageSavingArgs](../pagesavingargs/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


