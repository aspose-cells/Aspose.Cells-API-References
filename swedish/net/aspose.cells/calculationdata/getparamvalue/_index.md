---
title: "CalculationData.GetParamValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CalculationData‑metod. Hämtar det representerade värdeobjektet för parametern på ett givet index"
type: docs
url: /sv/net/aspose.cells/calculationdata/getparamvalue/
---
## CalculationData.GetParamValue method

Hämtar det representerade värdeobjektet för parametern på ett givet index.

```csharp
public object GetParamValue(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Index för parametern (0‑baserat) |

### Returvärde

Det beräknade värdet för parametern.

### Anmärkningar

För en parameter:

Om det är ett enkelt värde, returneras själva enkla värdet;

Om det är en referens, returneras ett ReferredArea-objekt;

Om det refererar till dataset med flera värden, returneras en array av objekt;

Om det är någon form av uttryck som måste beräknas, beräknas det i värdeläge och vanligtvis returneras ett enda värde enligt den aktuella cellens bas. Till exempel, om en parameter i D2:s formel är A:A+B:B, beräknas A2+B2 och returneras. Om parametern däremot har angivits i arrayläge (av [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) eller [`CustomFunctionDefinition`](../../formulaparseoptions/customfunctiondefinition/)), returneras en array (object[][]) vars element är A1+B1,A2+B2,....

### Exempel

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

### Se även

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


