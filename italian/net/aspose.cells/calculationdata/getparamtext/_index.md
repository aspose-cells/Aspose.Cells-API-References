---
title: "CalculationData.GetParamText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CalculationData. Restituisce il testo letterale del parametro all'indice specificato"
type: docs
url: /it/net/aspose.cells/calculationdata/getparamtext/
---
## CalculationData.GetParamText method

Ottiene il testo letterale del parametro all'indice specificato.

```csharp
public string GetParamText(int index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | Int32 | indice del parametro (base 0) |

### Valore di ritorno

testo letterale del parametro

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataMethodGetParamTextWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            sheet.Cells["A1"].Formula = "=SUM(INDIRECT(\"'Book2.xlsx'!Table1[#All]\"))";
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalcEngine();
            workbook.CalculateFormula(options);
        }
    }

    class CustomCalcEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                Console.WriteLine("SUM parameter: " + data.GetParamText(0));
            }
            else if (data.FunctionName == "INDIRECT")
            {
                Console.WriteLine("INDIRECT parameter: " + data.GetParamText(0));
            }
        }
    }
}
```

### Vedi anche

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


