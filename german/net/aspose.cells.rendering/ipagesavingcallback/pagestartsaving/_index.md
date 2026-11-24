---
title: "IPageSavingCallback.PageStartSaving"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IPageSavingCallback-Methode. Steuern/Anzeigen, dass eine Seite ausgegeben wird"
type: docs
url: /de/net/aspose.cells.rendering/ipagesavingcallback/pagestartsaving/
---
## IPageSavingCallback.PageStartSaving method

Steuert/zeigt den Beginn einer auszugebenden Seite an.

```csharp
public void PageStartSaving(PageStartSavingArgs args)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| args | PageStartSavingArgs | Info für den Beginn des Seiten‑Speichervorgangs. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class IPageSavingCallbackMethodPageStartSavingWithPageStartSavingArgsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispielinhalt hinzufügen, um mehrere Seiten zu erstellen
            for (int i = 0; i < 150; i++)
                worksheet.Cells[$"A{i + 1}"].Value = $"Data row {i + 1}";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PageSavingCallback callback = new PageSavingCallback();
            saveOptions.PageSavingCallback = callback;

            try
            {
                workbook.Save("PageStartSavingOutput.pdf", saveOptions);
                Console.WriteLine($"Processed pages: {callback.ProcessedPages}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class PageSavingCallback : IPageSavingCallback
    {
        public int ProcessedPages { get; private set; }

        public void PageStartSaving(PageStartSavingArgs args)
        {
            if (args.PageIndex % 3 == 0) // Skip every 3rd page (0-based)
                args.IsToOutput = false;
            else
                ProcessedPages++;

            Console.WriteLine(args.IsToOutput 
                ? $"Saving page {args.PageIndex + 1}"
                : $"Skipping page {args.PageIndex + 1}");
        }

        public void PageEndSaving(PageEndSavingArgs args)
        {
            // Optionale Behandlung des Seitenendes
        }
    }
}
```

### Siehe auch

* class [PageStartSavingArgs](../../pagestartsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


