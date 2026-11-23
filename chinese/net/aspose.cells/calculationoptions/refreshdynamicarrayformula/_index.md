---
title: "CalculationOptions.RefreshDynamicArrayFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CalculationOptions 属性。指示是否在计算公式之前刷新动态数组公式"
type: docs
url: /zh/net/aspose.cells/calculationoptions/refreshdynamicarrayformula/
---
## CalculationOptions.RefreshDynamicArrayFormula property

指示是否在计算公式之前刷新动态数组公式。

```csharp
public bool RefreshDynamicArrayFormula { get; set; }
```

### 备注

如果显式指定了此属性，则使用指定的值来决定是否刷新动态数组公式。否则（[`UserSpecifiedRefreshDynamicArrayFormula`](../userspecifiedrefreshdynamicarrayformula/) 为 false），其默认值取决于需要计算的公式类型：对于工作簿的公式计算，例如 [`CalculateFormula`](../../workbook/calculateformula/)，此属性将视为 true。对于其他情况，例如 [`Calculate`](../../cell/calculate/) 或 [`CalculateFormula`](../../worksheet/calculateformula/)，此属性将视为 false。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一个动态数组公式以演示其功能
            worksheet.Cells["A1"].Value = 1;
            worksheet.Cells["A2"].Value = 2;
            worksheet.Cells["A3"].Value = 3;
            worksheet.Cells["B1"].Formula = "=A1:A3"; // Dynamic array formula

            // 创建 CalculationOptions 实例
            CalculationOptions options = new CalculationOptions();

            try
            {
                // 显示 RefreshDynamicArrayFormula 的默认值
                Console.WriteLine("Default RefreshDynamicArrayFormula value: " + options.RefreshDynamicArrayFormula);

                // 将属性设置为 true 以刷新动态数组公式
                options.RefreshDynamicArrayFormula = true;
                Console.WriteLine("After setting to true: " + options.RefreshDynamicArrayFormula);

                // 使用指定的选项计算公式
                workbook.CalculateFormula(options);

                // 显示计算结果
                Console.WriteLine("Dynamic array formula result: " + worksheet.Cells["B1"].Value);

                // 保存工作簿
                workbook.Save("RefreshDynamicArrayFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


