---
title: "Enum CalculationPrecisionStrategy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CalculationPrecisionStrategy‑enum. Enumererar strategier för att hantera beräkningsprecision. På grund av precisionproblemet i IEEE 754 FloatingPoint Arithmetic kan vissa till synes enkla formler inte beräknas till det förväntade resultatet. Till exempel formeln 0.450.430.02 när operander beräknas med operatorn direkt ger resultatet inte noll. För sådana precisionproblem kan vissa speciella strategier ge det förväntade resultatet"
type: docs
url: /sv/net/aspose.cells/calculationprecisionstrategy/
---
## CalculationPrecisionStrategy enumeration

Enumererar strategier för att hantera beräkningsprecision. På grund av precisionproblemet i IEEE 754 flyttalsaritmetik kan vissa \"till synes enkla\" formler inte beräknas till det förväntade resultatet. Till exempel formeln \"=-0.45+0.43+0.02\", när operander beräknas med '+'-operatorn direkt, blir resultatet inte noll. För den här typen av precisionproblem kan vissa speciella strategier ge det förväntade resultatet.

```csharp
public enum CalculationPrecisionStrategy
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen strategi tillämpas vid beräkning. Vid beräkning används bara det ursprungliga dubbelvärdet som operand och resultatet returneras direkt. Mest effektivt för prestanda och tillämpligt i de flesta fall. |
| Round | `1` | Avrundar beräkningsresultatet enligt signifikanta siffror. |
| Decimal | `2` | Använder decimal som operand när det är möjligt. Mest ineffektivt för prestanda. |

### Exempel

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CalculationPrecisionStrategyDemo
    {
        public static void CalculationPrecisionStrategyExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Formula");
            worksheet.Cells["A2"].Formula = "=-0.45+0.43+0.02"; // This should ideally equal 0

            // Ställ in beräkningsalternativ
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                PrecisionStrategy = CalculationPrecisionStrategy.Round // Using Round strategy
            };

            // Beräkna formlerna i kalkylbladet
            workbook.CalculateFormula(calcOptions);

            // Hämta resultatet av formeln
            double result = worksheet.Cells["A2"].DoubleValue;

            // Skriv ut resultatet
            Console.WriteLine("Calculated Result: " + result);

            // Spara arbetsboken
            workbook.Save("CalculationPrecisionStrategyExample.xlsx");
            workbook.Save("CalculationPrecisionStrategyExample.pdf");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


