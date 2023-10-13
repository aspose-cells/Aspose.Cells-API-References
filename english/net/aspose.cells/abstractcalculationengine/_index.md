---
title: Class AbstractCalculationEngine
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.AbstractCalculationEngine class. Represents users custom calculation engine to extend the default calculation engine of Aspose.Cells
type: docs
url: /net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.

```csharp
public abstract class AbstractCalculationEngine
```

## Properties

| Name | Description |
| --- | --- |
| virtual [IsParamArrayModeRequired](../../aspose.cells/abstractcalculationengine/isparamarraymoderequired/) { get; } | Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If [`GetParamValueInArrayMode`](../calculationdata/getparamvalueinarraymode/) is required when calculating custom functions and user has not updated the definition for them (by [`UpdateCustomFunctionDefinition`](../workbook/updatecustomfunctiondefinition/)), this property needs to be set as true. |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired/) { get; } | Indicates whether this engine needs the literal text of parameter while doing calculation. Default value is false. |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions/) { get; } | Whether built-in functions that have been supported by the built-in engine should be checked and processed by this implementation. Default is false. |

## Methods

| Name | Description |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate/)(CalculationData) | Calculates one function with given data. |

### Remarks

User should not modify any part of the Workbook directly in this implementation(except the calculated result of the custom function, which can be set by CalculationData.CalculatedValue property). Otherwise unexpected result or Exception may be caused. If user needs to change other data than calculated result in the implementation for some custom functions, for example, change cell's formula, style, ...etc., user should gather those data in this implementation and change them out of the scope of formula calculation.

### Examples

```csharp
[C#]
Workbook wb = new Workbook("custom_calc.xlsx");
CalculationOptions opts = new CalculationOptions();
opts.CustomEngine = new MyEngine();
wb.CalculateFormula(opts);

class MyEngine : AbstractCalculationEngine
{
    public override void Calculate(CalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {
            //do calculation for MYFUNC here
            int count = data.ParamCount;
            object res = null;
            for (int i = 0; i < count; i++)
            {
                object pv = data.GetParamValue(i);
                if (pv is ReferredArea)
                {
                    ReferredArea ra = (ReferredArea)pv;
                    pv = ra.GetValue(0, 0);
                }
                //process the parameter here
                //res = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


