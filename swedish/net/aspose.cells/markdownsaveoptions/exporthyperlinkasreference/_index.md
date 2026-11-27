---
title: "MarkdownSaveOptions.ExportHyperlinkAsReference"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions‑egenskap. Anger om hyperlänken ska exporteras med referensdefinitioner istället för inbäddat format. Standardvärdet är falskt."
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/exporthyperlinkasreference/
---
## MarkdownSaveOptions.ExportHyperlinkAsReference property

Anger om hyperlänken ska exporteras med referensdefinitioner istället för inline-format. Standardvärdet är falskt.

```csharp
public bool ExportHyperlinkAsReference { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyExportHyperlinkAsReferenceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Placera en exempeltext i en cell
            sheet.Cells["A1"].PutValue("Visit Aspose");

            // Lägg till en hyperlänk i cellen (A1)
            // Parametrar: firstRow, firstColumn, totalRows, totalColumns, hyperlink
            sheet.Hyperlinks.Add(0, 0, 1, 1, "https://www.aspose.com");

            // Initiera Markdown‑sparalternativ
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Åtkomst direkt till ExportHyperlinkAsReference‑egenskapen (skrivskyddad i den här demonstrationen)
                Console.WriteLine("ExportHyperlinkAsReference value: " + saveOptions.ExportHyperlinkAsReference);

                // Spara arbetsboken som markdown; egenskapen (om true) påverkar hur hyperlänkar exporteras
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

### Se även

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


