---
title: AbstractCalculationEngine.IsParamArrayModeRequired
second_title: Aspose.Cells for .NET API Reference
description: AbstractCalculationEngine property. Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If GetParamValueInArrayMode is required when calculating custom functions and user has not updated the definition for them by UpdateCustomFunctionDefinition this property needs to be set as true
type: docs
url: /net/aspose.cells/abstractcalculationengine/isparamarraymoderequired/
---
## AbstractCalculationEngine.IsParamArrayModeRequired property

Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If [`GetParamValueInArrayMode`](../../calculationdata/getparamvalueinarraymode/) is required when calculating custom functions and user has not updated the definition for them (by [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/)), this property needs to be set as true.

```csharp
public virtual bool IsParamArrayModeRequired { get; }
```

### Remarks

If this custom calculation engine needs the parameter to be calculated in array mode, more stacks will be required to cache the tree for parameters and Calculate() method may be called recursively to calculate the parameter's value. For performance consideration, please keep this property as the default value(false) if there is no special requirement.

### Examples

```csharp
namespace AsposeCellsExamples.AbstractCalculationEnginePropertyIsParamArrayModeRequiredDemo
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
                    object param = data.GetParamValue(i);
                    if (param is Array arr)
                    {
                        foreach (object item in arr)
                        {
                            if (item is double d) sum += d;
                        }
                    }
                    else if (param is double d)
                    {
                        sum += d;
                    }
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

### See Also

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


