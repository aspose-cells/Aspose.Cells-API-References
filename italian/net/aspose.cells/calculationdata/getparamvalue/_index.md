---
title: "CalculationData.GetParamValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CalculationData. Ottiene l'oggetto valore rappresentato del parametro a un indice specificato"
type: docs
url: /it/net/aspose.cells/calculationdata/getparamvalue/
---
## CalculationData.GetParamValue method

Ottiene l'oggetto valore rappresentato del parametro a un dato indice.

```csharp
public object GetParamValue(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | L'indice del parametro (base 0) |

### Valore di ritorno

Il valore calcolato del parametro.

### Osservazioni

Per un parametro:

Se è un valore semplice, restituisce il valore semplice stesso;

Se è un riferimento, restituisce l'oggetto ReferredArea;

Se fa riferimento a dataset con più valori, restituisce un array di oggetti;

Se è una sorta di espressione che necessita di essere calcolata, verrà calcolata in modalità valore e generalmente verrà restituito un singolo valore in base alla cella corrente. Ad esempio, se un parametro della formula di D2 è A:A+B:B, allora A2+B2 verrà calcolato e restituito. Tuttavia, se questo parametro è stato specificato in modalità array (tramite [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) o [`CustomFunctionDefinition`](../../formulaparseoptions/customfunctiondefinition/)), verrà restituito un array (object[][]) i cui elementi sono A1+B1,A2+B2,....

### Esempi

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

### Vedi anche

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


