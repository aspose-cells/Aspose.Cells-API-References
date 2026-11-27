---
title: "CalculationOptions.IgnoreError"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationOptions-egenskapen. Anger om fel som uppstår vid beräkning av formler ska ignoreras. Felet kan vara en funktion som inte stöds, externa länkar etc. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/calculationoptions/ignoreerror/
---
## CalculationOptions.IgnoreError property

Anger om fel som uppstår vid beräkning av formler ska ignoreras. Felet kan vara en funktion som inte stöds, externa länkar osv. Standardvärdet är true.

```csharp
public bool IgnoreError { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett namngivet område som inte finns för att demonstrera felhantering
            worksheet.Cells["A1"].Formula = "=NONEXISTENTNAME()";
            
            // Beräkna med IgnoreError = false (kommer att kasta fel)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = false });
                Console.WriteLine("Calculation completed without ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (expected): " + ex.Message);
            }

            // Beräkna med IgnoreError = true (kommer att undertrycka fel)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = true });
                Console.WriteLine("Calculation completed while ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (unexpected): " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


