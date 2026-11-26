---
title: "CalculationOptions.CustomEngine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CalculationOptions. El motor de cálculo de fórmulas personalizado para ampliar el motor de cálculo predeterminado de Aspose.Cells"
type: docs
url: /es/net/aspose.cells/calculationoptions/customengine/
---
## CalculationOptions.CustomEngine property

El motor de cálculo de fórmulas personalizado para ampliar el motor de cálculo predeterminado de Aspose.Cells.

```csharp
public AbstractCalculationEngine CustomEngine { get; set; }
```

### Ejemplos

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
            
            // Establecer la fórmula HYPERLINK en la celda A1
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://example.com\",\"Click Here\")";
            
            // Crear un motor personalizado que procese la función HYPERLINK
            CustomEngineForHyperlink customEngine = new CustomEngineForHyperlink(true);
            
            // Establecer opciones de cálculo con motor personalizado
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = customEngine;
            
            // Calcule fórmulas con el motor personalizado
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
            // No llame a base.Calculate() ya que es abstracto
            // Simplemente permita que el cálculo predeterminado ocurra para otras funciones
        }
    }
}
```

### Ver también

* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


