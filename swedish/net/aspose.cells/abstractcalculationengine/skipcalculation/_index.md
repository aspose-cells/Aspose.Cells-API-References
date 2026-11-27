---
title: "AbstractCalculationEngine.SkipCalculation"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractCalculationEngine-metod. Hoppar över beräkningen för hela formeln som refererar till funktionen som för närvarande utvärderas"
type: docs
url: /sv/net/aspose.cells/abstractcalculationengine/skipcalculation/
---
## AbstractCalculationEngine.SkipCalculation method

Hoppar över beräkningen för hela formeln som refererar till funktionen som för närvarande utvärderas.

```csharp
public void SkipCalculation()
```

### Anmärkningar

Denna metod kan anropas i implementationen av [`Calculate`](../calculate/) för att hoppa över beräkningen av hela formeln och det ursprungliga värdet av formeln kommer att behållas utan förändring.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodSkipCalculationDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data för sammanhang
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Formula = "=SKIPFUNC(A1,A2)";

            // Skapa anpassad beräkningsmotor
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomSkipEngine();

            try
            {
                // Beräkna arbetsboken som kommer att trigga vår anpassade motor
                workbook.CalculateFormula(options);

                // Visa resultatet (bör hoppas över)
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].StringValue);

                // Spara arbetsboken
                workbook.Save("SkipCalculationDemo.xlsx");
                Console.WriteLine("SkipCalculation method demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SkipCalculation: {ex.Message}");
            }
        }
    }

    public class CustomSkipEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.ToUpper() == "SKIPFUNC")
            {
                // Hoppa över beräkningen för denna formel
                SkipCalculation();
                data.CalculatedValue = "#SKIPPED!";
            }
        }
    }
}
```

### Se även

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


