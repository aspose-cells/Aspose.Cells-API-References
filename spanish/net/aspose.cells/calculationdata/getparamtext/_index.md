---
title: "CalculationData.GetParamText"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CalculationData. Obtiene el texto literal del parámetro en el índice dado"
type: docs
url: /es/net/aspose.cells/calculationdata/getparamtext/
---
## CalculationData.GetParamText method

Obtiene el texto literal del parámetro en el índice dado.

```csharp
public string GetParamText(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | índice del parámetro (basado en 0) |

### Valor de retorno

texto literal del parámetro

### Ejemplos

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

### Ver también

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


