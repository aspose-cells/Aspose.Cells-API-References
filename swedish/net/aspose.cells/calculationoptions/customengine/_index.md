---
title: "CalculationOptions.CustomEngine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationOptions-egenskapen. Den anpassade formelberäkningsmotorn för att utöka standardberäkningsmotorn i Aspose.Cells"
type: docs
url: /sv/net/aspose.cells/calculationoptions/customengine/
---
## CalculationOptions.CustomEngine property

Den anpassade formelberäkningsmotorn för att utöka standardberäkningsmotorn i Aspose.Cells.

```csharp
public AbstractCalculationEngine CustomEngine { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCustomEngineDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ställ in HYPERLINK-formeln i cell A1
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://example.com\",\"Click Here\")";
            
            // Skapa en anpassad motor som bearbetar HYPERLINK-funktionen
            CustomEngineForHyperlink customEngine = new CustomEngineForHyperlink(true);
            
            // Ställ in beräkningsalternativ med anpassad motor
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = customEngine;
            
            // Beräkna formler med den anpassade motorn
            wb.CalculateFormula(options);
            
            Console.WriteLine("Custom engine invoked: " + customEngine.Invoked);
        }
    }

    public class CustomEngineForHyperlink : AbstractCalculationEngine
    {
        public bool Invoked { get; private set; }
        private readonly bool _shouldProcess;

        public CustomEngineForHyperlink(bool shouldProcess)
        {
            _shouldProcess = shouldProcess;
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "HYPERLINK" && _shouldProcess)
            {
                Invoked = true;
                data.CalculatedValue = "[Custom Processed] " + data.GetParamText(1);
            }
            // Anropa inte base.Calculate() eftersom den är abstrakt
            // Låt bara standardberäkningen ske för andra funktioner
        }
    }
}
```

### Se även

* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


