---
title: "MarkdownSaveOptions.ExportHyperlinkAsReference"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownSaveOptions‑Eigenschaft. Gibt an, ob Hyperlinks mithilfe von Referenzdefinitionen anstelle des Inline‑Formats exportiert werden. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/exporthyperlinkasreference/
---
## MarkdownSaveOptions.ExportHyperlinkAsReference property

Gibt an, ob Hyperlinks mithilfe von Referenzdefinitionen anstelle des Inline-Formats exportiert werden sollen. Der Standardwert ist false.

```csharp
public bool ExportHyperlinkAsReference { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportHyperlinkAsReferenceDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge einen Beispieltext in eine Zelle ein
            sheet.Cells["A1"].PutValue("Visit Aspose");

            // Füge einen Hyperlink zur Zelle (A1) hinzu
            // Parameter: firstRow, firstColumn, totalRows, totalColumns, hyperlink
            sheet.Hyperlinks.Add(0, 0, 1, 1, "https://www.aspose.com");

            // Initialisiere Markdown‑Speicheroptionen
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Greife direkt auf die ExportHyperlinkAsReference‑Eigenschaft zu (schreibgeschützt in dieser Demo)
                Console.WriteLine("ExportHyperlinkAsReference value: " + saveOptions.ExportHyperlinkAsReference);

                // Speichere die Arbeitsmappe als Markdown; die Eigenschaft (wenn true) beeinflusst, wie Hyperlinks exportiert werden
                workbook.Save("ExportHyperlinkAsReferenceDemo.md", saveOptions);
                Console.WriteLine("Workbook saved as markdown.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


