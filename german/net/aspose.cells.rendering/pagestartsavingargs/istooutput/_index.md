---
title: "PageStartSavingArgs.IsToOutput"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageStartSavingArgs-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob die Seite ausgegeben werden soll. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells.rendering/pagestartsavingargs/istooutput/
---
## PageStartSavingArgs.IsToOutput property

Liest oder setzt einen Wert, der angibt, ob die Seite ausgegeben werden soll. Der Standardwert ist true.

```csharp
public bool IsToOutput { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageStartSavingArgsPropertyIsToOutputDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Daten füllen, um mehrere Seiten zu erstellen
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
                // Korrigiert: Zeilenhöhe über die Rows-Sammlung des Arbeitsblatts zugreifen
                worksheet.Cells.Rows[i].Height = 50;
            }

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            workbook.Save("PageOutputDemo.pdf", saveOptions);
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // Aktuellen Wert lesen
                Console.WriteLine($"Page {args.PageIndex + 1} - Initial IsToOutput: {args.IsToOutput}");

                // Jede gerade nummerierte Seite überspringen (1-basierte Nummerierung)
                if ((args.PageIndex + 1) % 2 == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine($"Disabling output for page {args.PageIndex + 1}");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // Implementierung für diese Demonstration nicht erforderlich
            }
        }
    }
}
```

### Siehe auch

* class [PageStartSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


