---
title: "Interface IPageSavingCallback"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.IPageSavingCallback‑Schnittstelle. Steuert/zeigt den Fortschritt des Seiten‑Speichervorgangs an."
type: docs
url: /de/net/aspose.cells.rendering/ipagesavingcallback/
---
## IPageSavingCallback interface

Steuern/Anzeigen des Fortschritts des Seiten‑Speichervorgangs.

```csharp
public interface IPageSavingCallback
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [PageEndSaving](../../aspose.cells.rendering/ipagesavingcallback/pageendsaving/)(PageEndSavingArgs) | Steuert/zeigt das Ende einer auszugebenden Seite an. |
| [PageStartSaving](../../aspose.cells.rendering/ipagesavingcallback/pagestartsaving/)(PageStartSavingArgs) | Steuert/zeigt den Beginn einer auszugebenden Seite an. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingCallbackDemo : IPageSavingCallback
    {
        public static void PageSavingCallbackExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // Erstelle Speicheroptionen mit einem Seiten‑Speicher‑Callback
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.PageSavingCallback = new PageSavingCallbackDemo();

            // Speichere die Arbeitsmappe als DOCX‑Datei
            workbook.Save("PageSavingCallbackExample.docx", saveOptions);
        }

        // Implementiere die Methode PageStartSaving
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }

        // Implementiere die Methode PageEndSaving
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


