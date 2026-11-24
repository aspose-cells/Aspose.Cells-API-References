---
title: "CalculationOptions.CustomEngine"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationOptions-Eigenschaft. Die benutzerdefinierte Formelberechnungs-Engine, um die Standardberechnungs-Engine von Aspose.Cells zu erweitern."
type: docs
url: /de/net/aspose.cells/calculationoptions/customengine/
---
## CalculationOptions.CustomEngine property

Die benutzerdefinierte Formelberechnungs‑Engine, um die Standard‑Berechnungs‑Engine von Aspose.Cells zu erweitern.

```csharp
public AbstractCalculationEngine CustomEngine { get; set; }
```

### Beispiele

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
            
            // Setzen Sie die HYPERLINK-Formel in Zelle A1
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://example.com\",\"Click Here\")";
            
            // Erstellen Sie eine benutzerdefinierte Engine, die die HYPERLINK-Funktion verarbeitet
            CustomEngineForHyperlink customEngine = new CustomEngineForHyperlink(true);
            
            // Setzen Sie die Berechnungsoptionen mit benutzerdefinierter Engine
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = customEngine;
            
            // Formeln mit der benutzerdefinierten Engine berechnen
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
            // Rufen Sie base.Calculate() nicht auf, da es abstrakt ist
            // Lassen Sie die Standardberechnung für andere Funktionen einfach stattfinden
        }
    }
}
```

### Siehe auch

* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


