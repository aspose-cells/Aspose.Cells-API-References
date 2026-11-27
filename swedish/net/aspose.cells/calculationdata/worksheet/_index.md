---
title: "CalculationData.Worksheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationData-egenskap. Hämtar Worksheet-objektet där funktionen finns"
type: docs
url: /sv/net/aspose.cells/calculationdata/worksheet/
---
## CalculationData.Worksheet property

Hämtar Worksheet-objektet där funktionen är.

```csharp
public Worksheet Worksheet { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorksheetDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Lägg till data för att göra exemplet meningsfullt
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Skapa beräkningsalternativ med anpassad motor
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new WorksheetDemoEngine();

                // Beräkna formler med alternativ
                workbook.CalculateFormula(options);

                // Visa resultatet
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Spara resultatet
                workbook.Save("WorksheetDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class WorksheetDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Åtkomst till den skrivskyddade Worksheet-egenskapen
                Worksheet worksheet = data.Worksheet;
                Console.WriteLine($"Function is in worksheet: {worksheet.Name}");

                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### Se även

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


