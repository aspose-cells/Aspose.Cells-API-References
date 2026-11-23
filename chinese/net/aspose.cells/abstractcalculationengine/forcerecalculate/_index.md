---
title: "AbstractCalculationEngine.ForceRecalculate"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AbstractCalculationEngine 方法。是否在计算共享公式时始终强制重新计算给定函数"
type: docs
url: /zh/net/aspose.cells/abstractcalculationengine/forcerecalculate/
---
## AbstractCalculationEngine.ForceRecalculate method

是否在计算共享公式时始终强制重新计算给定函数。

```csharp
public virtual bool ForceRecalculate(string functionName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| functionName | String | 函数的名称。通常是自定义函数的名称。如果 [`ProcessBuiltInFunctions`](../processbuiltinfunctions/) 为 true，则内置函数也将在此检查。 |

### 返回值

如果指定的函数需要始终重新计算，则为 true。

### 备注

对于共享公式，多个单元格共享同一个函数。如果这些单元格的函数参数保持相同，通常该函数只需计算一次。因此出于性能考虑，我们也只会计算此类函数一次（[`Calculate`](../calculate/) 只会被调用一次，而不是对每个单元格重复调用）。然而，对于用户的自定义实现，函数，尤其是自定义函数，可能需要对不同单元格进行不同的计算。如果是这种情况，用户需要覆盖此方法，使其对该函数返回 true。并且对于 [`Calculate`](../calculate/)，给定的 [`CalculatedValue`](../../calculationdata/calculatedvalue/) 可能已经使用上一次计算的缓存值进行初始化。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;


    public class AbstractCalculationEngineMethodForceRecalculateWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            MyCustomEngine engine = new MyCustomEngine();
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = engine;

            worksheet.Cells["A1"].Formula = "MYVOLATILEFUNC()";

            try
            {
                bool result = engine.ForceRecalculate("MYVOLATILEFUNC");
                Console.WriteLine($"ForceRecalculate returned: {result} for 'MYVOLATILEFUNC'");

                workbook.CalculateFormula(options);
                Console.WriteLine($"First calculation result: {worksheet.Cells["A1"].Value}");

                System.Threading.Thread.Sleep(1000);
                workbook.CalculateFormula(options);
                Console.WriteLine($"Second calculation result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ForceRecalculate: {ex.Message}");
            }

            workbook.Save("ForceRecalculateDemo.xlsx");
        }
    }


    public class MyCustomEngine : AbstractCalculationEngine
    {
        private int calculationCount = 0;

        public override bool ForceRecalculate(string functionName)
        {
            return functionName == "MYVOLATILEFUNC";
        }

        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYVOLATILEFUNC")
            {
                calculationCount++;
                data.CalculatedValue = calculationCount;
            }
        }
    }
}
```

### 另请参见

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


