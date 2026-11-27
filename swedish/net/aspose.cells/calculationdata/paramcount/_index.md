---
title: "CalculationData.ParamCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationData‑egenskap. Hämtar antalet parametrar"
type: docs
url: /sv/net/aspose.cells/calculationdata/paramcount/
---
## CalculationData.ParamCount property

Hämtar antalet parametrar

```csharp
public int ParamCount { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyParamCountDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny arbetsbok och hämta det första kalkylbladet
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Fyll i några celler som kommer att användas som parametrar
                sheet.Cells["A1"].PutValue(10);
                sheet.Cells["A2"].PutValue(20);
                sheet.Cells["A3"].PutValue(30);

                // Ange en formel som anropar en anpassad funktion med tre argument
                sheet.Cells["B1"].Formula = "=DEMOPARAM(A1, A2, A3)";

                // Konfigurera beräkningsalternativ för att använda en anpassad motor
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ParamCountEngine();

                // Utför beräkning
                workbook.CalculateFormula(options);

                // Den anpassade motorn returnerar ParamCount som det beräknade värdet
                Console.WriteLine("ParamCount reported by custom function: " + sheet.Cells["B1"].Value);
                
                // Spara arbetsboken valfritt
                workbook.Save("ParamCountDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Anpassad beräkningsmotor som demonstrerar läsning av ParamCount‑egenskapen
        private class ParamCountEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Identifiera den anpassade funktionen efter namn
                if (data.FunctionName != null && data.FunctionName.Equals("DEMOPARAM", StringComparison.OrdinalIgnoreCase))
                {
                    // Läs den skrivskyddade ParamCount‑egenskapen
                    int count = data.ParamCount;

                    // Använd antalet som resultatet av funktionen
                    data.CalculatedValue = count;
                }
            }
        }
    }
}
```

### Se även

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


