---
title: "PdfSaveOptions.EmbedStandardWindowsFonts"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions Eigenschaft. True, um TrueType-Schriften einzubetten. Betrifft nur ASCII‑Zeichen 32127. Schriften für Zeichen­codes größer als 127 werden immer eingebettet. Schriften werden für den PDF/A‑1a‑ und PDF/A‑1b‑Standard immer eingebettet. Standard ist true."
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/embedstandardwindowsfonts/
---
## PdfSaveOptions.EmbedStandardWindowsFonts property

True, um TrueType-Schriften einzubetten. Betrifft nur ASCII‑Zeichen 32‑127. Schriften für Zeichen­codes größer als 127 werden immer eingebettet. Schriften werden für den PDF/A‑1a‑ und PDF/A‑1b‑Standard immer eingebettet. Der Standardwert ist true.

```csharp
public bool EmbedStandardWindowsFonts { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyEmbedStandardWindowsFontsDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF with embedded fonts");

            // PDF‑Speicheroptionen mit der Eigenschaft EmbedStandardWindowsFonts festlegen
            PdfSaveOptions options = new PdfSaveOptions();
            options.EmbedStandardWindowsFonts = true;

            // In den Speicherstream speichern
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved with embedded fonts: " + (ms.Length > 0));
            }

            // Demonstration der Deaktivierung der Schriftart‑Einbettung
            options.EmbedStandardWindowsFonts = false;
            using (MemoryStream ms = new MemoryStream())
            {
                workbook.Save(ms, options);
                Console.WriteLine("PDF saved without embedded fonts: " + (ms.Length > 0));
            }
        }
    }
}
```

### Siehe auch

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


