---
title: "CalculationData.CalculatedValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationData‑egenskap. Hämtar eller anger det beräknade värdet för denna funktion"
type: docs
url: /sv/net/aspose.cells/calculationdata/calculatedvalue/
---
## CalculationData.CalculatedValue property

Hämtar eller anger det beräknade värdet för denna funktion.

```csharp
public object CalculatedValue { get; set; }
```

### Anmärkningar

Användaren bör ange den här egenskapen i sin anpassade beräkningsmotor för de funktioner som motorn stöder, och det angivna värdet kommer att returneras när egenskapen hämtas senare. Det angivna värdet kan vara av möjliga typer av [`Value`](../../cell/value/), eller en array av sådana värden, eller ett Range, Name, ReferredArea. Att hämta den här egenskapen innan ett värde har satts kommer att göra att funktionen beräknas av Aspose.Cells standardberäkningsmotor och sedan returneras det beräknade värdet (vanligtvis bör det vara #NAME? för användardefinierade funktioner).

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Skapa beräkningsalternativ med anpassad motor
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalculationEngine();

            // Beräkna formler med alternativ
            workbook.CalculateFormula(options);

            // Hämta det beräknade värdet
            Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
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

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


