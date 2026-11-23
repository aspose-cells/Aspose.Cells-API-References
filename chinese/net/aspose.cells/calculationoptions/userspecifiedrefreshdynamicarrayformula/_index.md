---
title: "CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CalculationOptions 属性。指示用户是否已明确指定在计算指定公式之前刷新动态数组公式的行为"
type: docs
url: /zh/net/aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/
---
## CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula property

指示用户是否已明确指定在计算指定公式之前刷新动态数组公式的行为。

```csharp
public bool UserSpecifiedRefreshDynamicArrayFormula { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyUserSpecifiedRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建示例工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些数据以使示例更有意义
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // 创建 CalculationOptions 实例
                CalculationOptions options = new CalculationOptions();

                // 显示 UserSpecifiedRefreshDynamicArrayFormula 属性的当前值
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula value: " +
                    options.UserSpecifiedRefreshDynamicArrayFormula);

                // 展示该属性如何影响行为
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula has been demonstrated");

                // 保存结果
                workbook.Save("UserSpecifiedRefreshDynamicArrayFormulaDemo.xlsx");
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


