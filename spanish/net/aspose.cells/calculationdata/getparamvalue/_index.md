---
title: "CalculationData.GetParamValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CalculationData. Obtiene el objeto de valor representado del parámetro en un índice dado"
type: docs
url: /es/net/aspose.cells/calculationdata/getparamvalue/
---
## CalculationData.GetParamValue method

Obtiene el objeto de valor representado del parámetro en un índice dado.

```csharp
public object GetParamValue(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice del parámetro (basado en 0) |

### Valor de retorno

El valor calculado del parámetro.

### Observaciones

Para un parámetro:

Si es un valor simple, entonces devuelve el propio valor simple;

Si es una referencia, entonces devuelve el objeto ReferredArea;

Si hace referencia a conjunto(s) de datos con múltiples valores, entonces devuelve una matriz de objetos;

Si es algún tipo de expresión que necesita ser calculada, entonces se calculará en modo valor y generalmente se devolverá un solo valor según la base de la celda actual. Por ejemplo, si un parámetro de la fórmula D2 es A:A+B:B, entonces A2+B2 se calculará y devolverá. Sin embargo, si este parámetro se ha especificado en modo matriz (por [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) o [`CustomFunctionDefinition`](../../formulaparseoptions/customfunctiondefinition/)), entonces se devolverá una matriz (object[][]) cuyos elementos son A1+B1,A2+B2,....

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataMethodGetParamValueWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=HYPERLINK(\"http://localhost:9090\", \"Target\")";

            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new HyperlinkCalculationEngine();
            workbook.CalculateFormula(options);
        }

        class HyperlinkCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName.Equals("HYPERLINK", StringComparison.OrdinalIgnoreCase))
                {
                    Console.WriteLine("URL Parameter: " + data.GetParamValue(0));
                    Console.WriteLine("Display Text: " + data.GetParamValue(1));
                }
            }
        }
    }
}
```

### Ver también

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


