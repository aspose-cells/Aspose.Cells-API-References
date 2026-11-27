---
title: "CalculationOptions.RefreshDynamicArrayFormula"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationOptions-egenskap. Anger om dynamiska array-formler ska uppdateras innan formler beräknas"
type: docs
url: /sv/net/aspose.cells/calculationoptions/refreshdynamicarrayformula/
---
## CalculationOptions.RefreshDynamicArrayFormula property

Anger om dynamiska matrisformler ska uppdateras innan formler beräknas.

```csharp
public bool RefreshDynamicArrayFormula { get; set; }
```

### Anmärkningar

Om denna egenskap har angetts explicit, kommer det angivna värdet att användas för att bestämma om dynamiska array-formler ska uppdateras. Annars([`UserSpecifiedRefreshDynamicArrayFormula`](../userspecifiedrefreshdynamicarrayformula/) är falskt), beror standardvärdet på vilken typ av formler som behöver beräknas: För beräkning av formler för arbetsboken, såsom [`CalculateFormula`](../../workbook/calculateformula/), kommer denna egenskap att betraktas som true. För andra fall, såsom [`Calculate`](../../cell/calculate/) eller [`CalculateFormula`](../../worksheet/calculateformula/), kommer denna egenskap att betraktas som false.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en dynamisk array-formel för att demonstrera funktionaliteten
            worksheet.Cells["A1"].Value = 1;
            worksheet.Cells["A2"].Value = 2;
            worksheet.Cells["A3"].Value = 3;
            worksheet.Cells["B1"].Formula = "=A1:A3"; // Dynamic array formula

            // Skapa en CalculationOptions-instans
            CalculationOptions options = new CalculationOptions();

            try
            {
                // Visa standardvärdet för RefreshDynamicArrayFormula
                Console.WriteLine("Default RefreshDynamicArrayFormula value: " + options.RefreshDynamicArrayFormula);

                // Ställ in egenskapen till true för att uppdatera dynamiska array-formler
                options.RefreshDynamicArrayFormula = true;
                Console.WriteLine("After setting to true: " + options.RefreshDynamicArrayFormula);

                // Beräkna formler med de angivna alternativen
                workbook.CalculateFormula(options);

                // Visa det beräknade resultatet
                Console.WriteLine("Dynamic array formula result: " + worksheet.Cells["B1"].Value);

                // Spara arbetsboken
                workbook.Save("RefreshDynamicArrayFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


