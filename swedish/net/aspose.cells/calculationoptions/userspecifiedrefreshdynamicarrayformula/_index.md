---
title: "CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationOptions-egenskap. Anger om användaren har uttryckligen specificerat beteendet för att uppdatera dynamiska matrisformler innan angivna formler beräknas"
type: docs
url: /sv/net/aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/
---
## CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula property

Anger om användaren uttryckligen har specificerat beteendet för att uppdatera dynamiska matrisformler innan angivna formler beräknas.

```csharp
public bool UserSpecifiedRefreshDynamicArrayFormula { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyUserSpecifiedRefreshDynamicArrayFormulaDemo
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
                // Skapa en CalculationOptions-instans
                CalculationOptions options = new CalculationOptions();

                // Visa det aktuella värdet av egenskapen UserSpecifiedRefreshDynamicArrayFormula
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula value: " +
                    options.UserSpecifiedRefreshDynamicArrayFormula);

                // Visa hur egenskapen påverkar beteendet
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula has been demonstrated");

                // Spara resultatet
                workbook.Save("UserSpecifiedRefreshDynamicArrayFormulaDemo.xlsx");
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

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


