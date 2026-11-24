---
title: "MarkdownSaveOptions.OfficeMathOutputType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownSaveOptions‑Eigenschaft. Gibt an, wie OfficeMath‑Objekte nach Markdown exportiert werden. Der Standardwert ist Image"
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/officemathoutputtype/
---
## MarkdownSaveOptions.OfficeMathOutputType property

Gibt an, wie OfficeMath‑Objekte nach Markdown exportiert werden. Der Standardwert ist Image.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputType { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten hinzu, einschließlich einer Formel, die OfficeMath enthalten könnte
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].Formula = "=SQRT(16)";

            try
            {
                // Erstelle Markdown‑Speicheroptionen
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Zeige den aktuellen Wert von OfficeMathOutputType an
                Console.WriteLine("Current OfficeMathOutputType: " + saveOptions.OfficeMathOutputType);

                // Setze OfficeMathOutputType auf MathML
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.MathML;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Speichere die Arbeitsmappe mit dem MathML‑Ausgabetyp
                workbook.Save("OfficeMathOutputType_MathML.md", saveOptions);

                // Wechsle zum Image‑Ausgabetyp
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.Image;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Speichere die Arbeitsmappe mit dem Image‑Ausgabetyp
                workbook.Save("OfficeMathOutputType_Image.md", saveOptions);

                Console.WriteLine("OfficeMathOutputType demonstration completed successfully.");
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

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


