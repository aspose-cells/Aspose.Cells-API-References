---
title: "AbstractCalculationEngine.SkipCalculation"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "AbstractCalculationEngine 方法。跳过对当前正在评估的函数所引用的整个公式的计算"
type: docs
url: /zh/net/aspose.cells/abstractcalculationengine/skipcalculation/
---
## AbstractCalculationEngine.SkipCalculation method

跳过对当前正在评估的函数所引用的整个公式的计算。

```csharp
public void SkipCalculation()
```

### 备注

此方法可在实现 [`Calculate`](../calculate/) 时调用，以跳过对整个公式的计算，公式的原始值将保持不变。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AbstractCalculationEngineMethodSkipCalculationDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些上下文数据
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Formula = "=SKIPFUNC(A1,A2)";

            // 创建自定义计算引擎
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomSkipEngine();

            try
            {
                // 计算工作簿以触发我们的自定义引擎
                workbook.CalculateFormula(options);

                // 显示结果（应跳过）
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].StringValue);

                // 保存工作簿
                workbook.Save("SkipCalculationDemo.xlsx");
                Console.WriteLine("SkipCalculation method demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SkipCalculation: {ex.Message}");
            }
        }
    }

    public class CustomSkipEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName.ToUpper() == "SKIPFUNC")
            {
                // 跳过此公式的计算
                SkipCalculation();
                data.CalculatedValue = "#SKIPPED!";
            }
        }
    }
}
```

### 另请参见

* class [AbstractCalculationEngine](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


