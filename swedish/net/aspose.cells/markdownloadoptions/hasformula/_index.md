---
title: "MarkdownLoadOptions.HasFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownLoadOptions-egenskap. Anger om texten är en formel om den börjar med"
type: docs
url: /sv/net/aspose.cells/markdownloadoptions/hasformula/
---
## MarkdownLoadOptions.HasFormula property

Anger om texten är en formel om den börjar med "=".

```csharp
public bool HasFormula { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en instans av MarkdownLoadOptions
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // Visa standardvärdet för HasFormula
                Console.WriteLine($"Default HasFormula value: {options.HasFormula}");

                // Ställ in HasFormula till true
                options.HasFormula = true;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Ställ in HasFormula till false
                options.HasFormula = false;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Skapa en arbetsbok med exempel på markdown-innehåll
                Workbook workbook = new Workbook();

                // Spara arbetsboken för att demonstrera att alternativen kan användas
                workbook.Save("HasFormulaDemo.xlsx");

                Console.WriteLine("HasFormula property demonstration completed successfully.");
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

* class [MarkdownLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


