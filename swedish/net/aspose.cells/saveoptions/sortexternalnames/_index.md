---
title: "SaveOptions.SortExternalNames"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Anger om externa definierade namn ska sorteras innan filen sparas"
type: docs
url: /sv/net/aspose.cells/saveoptions/sortexternalnames/
---
## SaveOptions.SortExternalNames property

Anger om externa definierade namn ska sorteras innan filen sparas.

```csharp
public bool SortExternalNames { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SaveOptionsPropertySortExternalNamesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Skapa en OoxmlSaveOptions-instans som ärver från SaveOptions
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Visa standardvärdet för SortExternalNames-egenskapen
                Console.WriteLine("Default SortExternalNames value: " + saveOptions.SortExternalNames);

                // Sätt SortExternalNames till true
                saveOptions.SortExternalNames = true;
                Console.WriteLine("SortExternalNames set to: " + saveOptions.SortExternalNames);

                // Spara arbetsboken med de angivna sparalternativen
                workbook.Save("SortExternalNamesDemo.xlsx", saveOptions);

                Console.WriteLine("Workbook saved with SortExternalNames enabled.");
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

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


