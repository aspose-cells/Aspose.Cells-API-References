---
title: "IPageSavingCallback.PageEndSaving"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IPageSavingCallback-Methode. Steuert/zeigt an, dass eine Seite beendet wird, um ausgegeben zu werden."
type: docs
url: /de/net/aspose.cells.rendering/ipagesavingcallback/pageendsaving/
---
## IPageSavingCallback.PageEndSaving method

Steuert/zeigt das Ende einer auszugebenden Seite an.

```csharp
public void PageEndSaving(PageEndSavingArgs args)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| args | PageEndSavingArgs | Informationen für eine Seite beenden den Speichervorgang. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class IPageSavingCallbackMethodPageEndSavingWithPageEndSavingArgsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und füllen Sie Daten ein.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu, um beim Rendern mehrere Seiten zu erzeugen.
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Row {i+1} - Demonstration data for page splitting";
            }

            // Erstellen Sie PDF-Speicheroptionen mit benutzerdefiniertem Seiten‑Speicher‑Callback.
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageEndSavingCallback();

            try
            {
                // Speichern Sie die Arbeitsmappe mit der Callback-Implementierung
                workbook.Save("PageEndSavingDemo.pdf", saveOptions);
                Console.WriteLine("Document saved successfully with page end tracking.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during document save: {ex.Message}");
            }
        }

        private class PageEndSavingCallback : IPageSavingCallback
        {
            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Anzeige der Abschlussinformationen zum Speichern der Seite
                Console.WriteLine($"Finished processing page {args.PageIndex + 1}");
                
                // Hier könnten Sie Dateioperationen oder andere Nachbearbeitungen hinzufügen
                // args.HasMorePages zeigt, ob weitere Seiten verarbeitet werden
            }

            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Erforderliche Schnittstellenimplementierung
            }
        }
    }
}
```

### Siehe auch

* class [PageEndSavingArgs](../../pageendsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


