---
title: "Range.ClearContents"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑metod. Rensar innehållet i detta område"
type: docs
url: /sv/net/aspose.cells/range/clearcontents/
---
## Range.ClearContents method

Rensar innehållet i detta område.

```csharp
public void ClearContents()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearContentsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att demonstrera rensning
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue("Sample");
            worksheet.Cells["B2"].PutValue("Data");

            try
            {
                // Skapa ett område som täcker cellerna A1:B2
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Visa områdets innehåll innan rensning
                Console.WriteLine("Before clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Anropa ClearContents för att ta bort alla värden i området
                range.ClearContents();

                // Visa områdets innehåll efter rensning
                Console.WriteLine("\nAfter clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Spara arbetsboken
                workbook.Save("ClearContentsDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
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

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


