---
title: "MarkdownSaveOptions.CalculateFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions-egenskap. Anger om formler ska beräknas innan markdown-filen sparas"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/calculateformula/
---
## MarkdownSaveOptions.CalculateFormula property

Anger om formler ska beräknas innan markdown‑filen sparas.

```csharp
public bool CalculateFormula { get; set; }
```

### Anmärkningar

Standardvärdet är falskt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med formler
            worksheet.Cells["A1"].PutValue("Price");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].Formula = "=A2*B2";

            try
            {
                // Skapa en instans av MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Visa standardvärdet för CalculateFormula
                Console.WriteLine("Default CalculateFormula value: " + saveOptions.CalculateFormula);

                // Ställ in CalculateFormula till true för att beräkna formler innan sparning
                saveOptions.CalculateFormula = true;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Spara arbetsboken med formelberäkning aktiverad
                workbook.Save("CalculateFormula_Enabled.md", saveOptions);

                // Ställ in CalculateFormula till false för att spara formler oförändrade
                saveOptions.CalculateFormula = false;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Spara arbetsboken med formelberäkning inaktiverad
                workbook.Save("CalculateFormula_Disabled.md", saveOptions);

                Console.WriteLine("CalculateFormula demonstration completed successfully.");
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


