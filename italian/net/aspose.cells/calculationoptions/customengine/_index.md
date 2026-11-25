---
title: "CalculationOptions.CustomEngine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CalculationOptions. Il motore di calcolo delle formule personalizzato per estendere il motore di calcolo predefinito di Aspose.Cells"
type: docs
url: /it/net/aspose.cells/calculationoptions/customengine/
---
## CalculationOptions.CustomEngine property

Il motore di calcolo delle formule personalizzato per estendere il motore di calcolo predefinito di Aspose.Cells.

```csharp
public AbstractCalculationEngine CustomEngine { get; set; }
```

### Esempi

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
            
            // Imposta la formula HYPERLINK nella cella A1
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://example.com\",\"Click Here\")";
            
            // Crea un motore personalizzato che elabora la funzione HYPERLINK
            CustomEngineForHyperlink customEngine = new CustomEngineForHyperlink(true);
            
            // Imposta le opzioni di calcolo con motore personalizzato
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = customEngine;
            
            // Calcola le formule con il motore personalizzato
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
            // Non chiamare base.Calculate() poiché è astratta
            // Lascia semplicemente che il calcolo predefinito avvenga per le altre funzioni
        }
    }
}
```

### Vedi anche

* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


