---
title: "MarkdownSaveOptions.AlignColumnPadding"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions egenskap. Anger om kolumnjustering är aktiverad för genererade Markdown-tabeller. När den är aktiverad justeras kolumner genom att fylla cellinnehållet med det angivna tecknet, vanligtvis mellanslag. Sätt till 0 för att inaktivera kolumnjustering (standard)"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/aligncolumnpadding/
---
## MarkdownSaveOptions.AlignColumnPadding property

Anger om kolumnjustering är aktiverad för genererade Markdown‑tabeller. När den är aktiverad justeras kolumnerna genom att fylla cellinnehållet med det angivna tecknet (vanligtvis ' ' för mellanslag). Ställ in på '\\0' för att inaktivera kolumnjustering (standard).

```csharp
public char AlignColumnPadding { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyAlignColumnPaddingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att demonstrera kolumnjustering
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "1.99";
            worksheet.Cells["C2"].Value = "10";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = "0.99";
            worksheet.Cells["C3"].Value = "20";

            // Skapa en instans av MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

            try
            {
                // Visa standardvärdet för AlignColumnPadding
                Console.WriteLine("Default AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Ställ in AlignColumnPadding till mellanslagstecken för kolumnjustering
                saveOptions.AlignColumnPadding = ' ';

                // Visa det uppdaterade värdet
                Console.WriteLine("Updated AlignColumnPadding value: '" +
                    saveOptions.AlignColumnPadding + "'");

                // Spara arbetsboken som markdown med kolumnjustering
                workbook.Save("AlignColumnPaddingDemo.md", saveOptions);
                Console.WriteLine("Markdown file saved with column alignment enabled.");
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


