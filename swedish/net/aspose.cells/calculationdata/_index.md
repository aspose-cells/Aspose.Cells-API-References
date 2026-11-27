---
title: "Klass CalculationData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CalculationData-klass. Representerar den erforderliga datan när en funktion beräknas, såsom funktionsnamn, parametrar ...etc"
type: docs
url: /sv/net/aspose.cells/calculationdata/
---
## CalculationData class

Representerar den nödvändiga datan vid beräkning av en funktion, såsom funktionsnamn, parametrar, ...etc.

```csharp
public class CalculationData
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CalculatedValue](../../aspose.cells/calculationdata/calculatedvalue/) { get; set; } | Hämtar eller anger det beräknade värdet för denna funktion. |
| [Cell](../../aspose.cells/calculationdata/cell/) { get; } | Hämtar Cell-objektet där funktionen är. |
| [CellColumn](../../aspose.cells/calculationdata/cellcolumn/) { get; } | Hämtar kolumnindexet för cellen där funktionen är. |
| [CellRow](../../aspose.cells/calculationdata/cellrow/) { get; } | Hämtar radindexet för cellen där funktionen är. |
| [FunctionName](../../aspose.cells/calculationdata/functionname/) { get; } | Hämtar funktionsnamnet som ska beräknas. |
| [ParamCount](../../aspose.cells/calculationdata/paramcount/) { get; } | Hämtar antalet parametrar |
| [Workbook](../../aspose.cells/calculationdata/workbook/) { get; } | Hämtar Workbook-objektet där funktionen är. |
| [Worksheet](../../aspose.cells/calculationdata/worksheet/) { get; } | Hämtar Worksheet-objektet där funktionen är. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetParamText](../../aspose.cells/calculationdata/getparamtext/)(int) | Hämtar den bokstavliga texten för parametern på det angivna indexet. |
| [GetParamValue](../../aspose.cells/calculationdata/getparamvalue/)(int) | Hämtar det representerade värdeobjektet för parametern på ett givet index. |
| [GetParamValueInArrayMode](../../aspose.cells/calculationdata/getparamvalueinarraymode/)(int, int, int) | Hämtar värdet/värdena för parametern på ett givet index. Om parametern är någon form av uttryck som måste beräknas, beräknas den i arrayläge. |

### Anmärkningar

Alla objekt som tillhandahålls av denna klass är endast avsedda för \"läs\"-ändamål. Användaren bör inte ändra någon data i Workbook under formelberäkningsprocessen, annars kan oväntade resultat eller undantag uppstå.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCalculationDataDemo
    {
        public static void Run()
        {
            try
            {
                // Förbered en enkel arbetsbok och arbetsblad
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Name = "DemoSheet";

                // Lägg in några värden som kommer att användas som parametrar i en anpassad funktion
                sheet.Cells["A1"].PutValue(5);
                sheet.Cells["A2"].PutValue(10);

                // Ställ in en formel som anropar den anpassade funktionen
                sheet.Cells["B1"].Formula = "=MYFUNC(A1, A2)";

                // Konfigurera beräkningsalternativ för att använda en anpassad motor
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new DemoEngine();

                // Utför beräkning – den anpassade motorn kommer att ta emot en CalculationData-instans
                workbook.CalculateFormula(options);

                // Skriv ut resultatet av den anpassade funktionen
                Console.WriteLine("Custom function result (B1): " + sheet.Cells["B1"].Value);

                // Spara arbetsboken för fullständighet
                workbook.Save("CalculationDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with CalculationData: {ex.Message}");
            }
        }

        // Anpassad beräkningsmotor som demonstrerar åtkomst till CalculationData-medlemmar
        private class DemoEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Säkerställ att vi hanterar den förväntade anpassade funktionen
                if (data.FunctionName != null &&
                    data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
                {
                    // Hämta parametervärden (de returneras som objekt)
                    object param0 = data.GetParamValue(0);
                    object param1 = data.GetParamValue(1);

                    // Konvertera parametrar till double för beräkning
                    double val0 = Convert.ToDouble(param0);
                    double val1 = Convert.ToDouble(param1);
                    double result = val0 + val1; // simple addition

                    // Tilldela det beräknade resultatet
                    data.CalculatedValue = result;

                    // Demonstrera läsning av skrivskyddade egenskaper
                    Console.WriteLine("[Engine] FunctionName : " + data.FunctionName);
                    Console.WriteLine("[Engine] ParamCount   : " + data.ParamCount);
                    Console.WriteLine("[Engine] CellRow      : " + data.CellRow);
                    Console.WriteLine("[Engine] CellColumn   : " + data.CellColumn);
                }
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


