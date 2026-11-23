---
title: "AbstractCalculationEngine.IsParamArrayModeRequired"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AbstractCalculationEngine 属性。指示此引擎是否需要在数组模式下计算参数。默认值为 false。如果在计算自定义函数时需要 GetParamValueInArrayMode 且用户尚未通过 UpdateCustomFunctionDefinition 更新其定义，则此属性需要设置为 true。"
type: docs
url: /zh/net/aspose.cells/abstractcalculationengine/isparamarraymoderequired/
---
## AbstractCalculationEngine.IsParamArrayModeRequired property

指示此引擎是否需要在数组模式下计算参数。默认值为 false。如果在计算自定义函数时需要 [`GetParamValueInArrayMode`](../../calculationdata/getparamvalueinarraymode/) 且用户尚未通过 [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) 更新其定义，则此属性需要设置为 true。

```csharp
public virtual bool IsParamArrayModeRequired { get; }
```

### 备注

如果此自定义计算引擎需要在数组模式下计算参数，则需要更多的栈来缓存参数的树，并且可能会递归调用 Calculate() 方法以计算参数的值。出于性能考虑，如果没有特殊需求，请保持此属性为默认值（false）。

### 示例

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

### 另请参见

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


