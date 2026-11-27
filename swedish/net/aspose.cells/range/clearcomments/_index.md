---
title: "Range.ClearComments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑metod. Rensar kommentarerna i detta område"
type: docs
url: /sv/net/aspose.cells/range/clearcomments/
---
## Range.ClearComments method

Rensar kommentarerna i detta område.

```csharp
public void ClearComments()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearCommentsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data och kommentarer i celler
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A1"].PutValue("This is a comment on A1", true, false);
            worksheet.Cells["B2"].Value = "More Data";
            worksheet.Cells["B2"].PutValue("This is a comment on B2", true, false);

            try
            {
                // Skapa ett område som inkluderar celler med kommentarer
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Rensa kommentarer från området
                range.ClearComments();

                Console.WriteLine("Comments cleared successfully from range A1:B2");
                Console.WriteLine($"Cell A1 value after clearing: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell B2 value after clearing: {worksheet.Cells["B2"].Value}");

                // Spara arbetsboken
                workbook.Save("ClearCommentsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearComments: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


