---
title: "Spinner.IsHorizontal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Spinner-egenskap. Anger om detta är en horisontell rullningslist"
type: docs
url: /sv/net/aspose.cells.drawing/spinner/ishorizontal/
---
## Spinner.IsHorizontal property

Anger om detta är en horisontell rullningslist.

```csharp
public bool IsHorizontal { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SpinnerPropertyIsHorizontalDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Lägg till en spinner-form i kalkylbladet
                Spinner spinner = worksheet.Shapes.AddSpinner(1, 0, 1, 0, 100, 30);
                
                // Ange spinner-egenskaper
                spinner.Min = 0;
                spinner.Max = 100;
                spinner.IncrementalChange = 5;
                spinner.CurrentValue = 50;
                
                // Demonstrera IsHorizontal-egenskapen (läsa och skriva)
                Console.WriteLine("Initial IsHorizontal value: " + spinner.IsHorizontal);
                
                // Växla orienteringen
                spinner.IsHorizontal = !spinner.IsHorizontal;
                Console.WriteLine("Modified IsHorizontal value: " + spinner.IsHorizontal);
                
                // Spara arbetsboken
                workbook.Save("SpinnerIsHorizontalDemo.xlsx");
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

* class [Spinner](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


