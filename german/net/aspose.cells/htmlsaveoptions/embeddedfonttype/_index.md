---
title: "HtmlSaveOptions.EmbeddedFontType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt den Typ der Einbettung von Schriftdateien in die HTML-Datei zurück oder legt ihn fest. Der Standardwert ist None, was bedeutet, dass keine Schriftart in HTML eingebettet wird"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/embeddedfonttype/
---
## HtmlSaveOptions.EmbeddedFontType property

Liest oder setzt den Typ der Einbettung von Schriftdateien in die HTML‑Datei. Standardwert ist None, was bedeutet, dass keine Schriftart in HTML eingebettet wird.

```csharp
public HtmlEmbeddedFontType EmbeddedFontType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample Text with Font");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);

            try
            {
                // HTML‑Speicheroptionen erstellen
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Zeigen Sie den Standardwert von EmbeddedFontType an
                Console.WriteLine("Default EmbeddedFontType: " + options.EmbeddedFontType);

                // Setzen Sie EmbeddedFontType auf Woff
                options.EmbeddedFontType = HtmlEmbeddedFontType.Woff;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Speichern Sie die Arbeitsmappe mit WOFF-Schriftart-Einbettung
                workbook.Save("EmbeddedFontType_Woff.html", options);

                // Zurücksetzen auf None
                options.EmbeddedFontType = HtmlEmbeddedFontType.None;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Arbeitsmappe ohne Schriftart-Einbettung speichern
                workbook.Save("EmbeddedFontType_None.html", options);

                Console.WriteLine("EmbeddedFontType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* enum [HtmlEmbeddedFontType](../../../aspose.cells.rendering/htmlembeddedfonttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


