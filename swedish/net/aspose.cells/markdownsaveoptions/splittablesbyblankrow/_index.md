---
title: "MarkdownSaveOptions.SplitTablesByBlankRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions-egenskap. Anger om tomma rader i kalkylbladet ska behandlas som tabellseparatorer vid export till Markdown. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/splittablesbyblankrow/
---
## MarkdownSaveOptions.SplitTablesByBlankRow property

Anger om tomma rader i arbetsbladet ska behandlas som tabellseparatorer vid export till Markdown. Standardvärdet är falskt.

```csharp
public bool SplitTablesByBlankRow { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertySplitTablesByBlankRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med tomma rader för att demonstrera tabelluppdelning
            worksheet.Cells["A1"].Value = "Table 1 Header";
            worksheet.Cells["B1"].Value = "Value 1";
            worksheet.Cells["A2"].Value = "Data 1";
            worksheet.Cells["B2"].Value = "Data 2";

            // Lägg till en tom rad (rad 3)
            worksheet.Cells["A4"].Value = "Table 2 Header";
            worksheet.Cells["B4"].Value = "Value 2";
            worksheet.Cells["A5"].Value = "Data 3";
            worksheet.Cells["B5"].Value = "Data 4";

            // Skapa en instans av MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Visa standardvärdet för SplitTablesByBlankRow
                Console.WriteLine("Default SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Ställ in SplitTablesByBlankRow till true för att dela tabeller vid tomma rader
                saveOptions.SplitTablesByBlankRow = true;

                // Visa det uppdaterade värdet
                Console.WriteLine("Updated SplitTablesByBlankRow value: " +
                    saveOptions.SplitTablesByBlankRow);

                // Spara arbetsboken som markdown med tabelluppdelning aktiverad
                workbook.Save("SplitTablesByBlankRowDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with table splitting by blank rows enabled.");
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


