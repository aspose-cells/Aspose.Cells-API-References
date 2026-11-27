---
title: "AbstractCalculationEngine.IsParamArrayModeRequired"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractCalculationEngine egenskap. Anger huruvida denna motor behöver parametern beräknas i array‑läge. Standardvärdet är false. Om GetParamValueInArrayMode krävs vid beräkning av anpassade funktioner och användaren inte har uppdaterat definitionen för dem med UpdateCustomFunctionDefinition, måste denna egenskap sättas till true."
type: docs
url: /sv/net/aspose.cells/abstractcalculationengine/isparamarraymoderequired/
---
## AbstractCalculationEngine.IsParamArrayModeRequired property

Anger huruvida denna motor behöver parametern beräknas i array‑läge. Standardvärdet är false. Om [`GetParamValueInArrayMode`](../../calculationdata/getparamvalueinarraymode/) krävs vid beräkning av anpassade funktioner och användaren inte har uppdaterat definitionen för dem (genom [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/)), måste denna egenskap sättas till true.

```csharp
public virtual bool IsParamArrayModeRequired { get; }
```

### Anmärkningar

Om denna anpassade beräkningsmotor behöver parametern beräknas i array‑läge, krävs fler stackar för att cachea trädstrukturen för parametrar och Calculate()-metoden kan anropas rekursivt för att beräkna parametervärdet. Av prestandaskäl, vänligen behåll denna egenskap med standardvärdet (false) om det inte finns något särskilt krav.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEnginePropertyIsParamArrayModeRequiredDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CustomCalculationEngine engine = new CustomCalculationEngine();
            Console.WriteLine("IsParamArrayModeRequired: " + engine.IsParamArrayModeRequired);

            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].Formula = "=SUMARRAY(A1,A2)";

            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;
            workbook.CalculateFormula(options);

            Console.WriteLine("SUMARRAY result: " + worksheet.Cells["A3"].Value);

            workbook.Save("IsParamArrayModeRequiredDemo.xlsx");
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override bool IsParamArrayModeRequired => true;

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUMARRAY")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(i);

                    double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));

                    sum += param1;
                }
                data.CalculatedValue = sum;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            return false;
        }
    }
}
```

### Se även

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


