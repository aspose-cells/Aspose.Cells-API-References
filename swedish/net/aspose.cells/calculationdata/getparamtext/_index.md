---
title: "CalculationData.GetParamText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationData‑metod. Hämtar den bokstavliga texten för parametern på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/calculationdata/getparamtext/
---
## CalculationData.GetParamText method

Hämtar den bokstavliga texten för parametern på det angivna indexet.

```csharp
public string GetParamText(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | index för parametern (0‑baserat) |

### Returvärde

bokstavlig text för parametern

### Exempel

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

### Se även

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


