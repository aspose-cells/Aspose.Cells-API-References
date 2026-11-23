---
title: "FormulaParseOptions.CustomFunctionDefinition"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FormulaParseOptions 属性。用于解析自定义函数的定义"
type: docs
url: /zh/net/aspose.cells/formulaparseoptions/customfunctiondefinition/
---
## FormulaParseOptions.CustomFunctionDefinition property

用于解析自定义函数的定义。

```csharp
public CustomFunctionDefinition CustomFunctionDefinition { get; set; }
```

### 备注

对于某些特殊需求，例如在用户自定义引擎中计算自定义函数时，其某些参数需要以数组模式计算，使用此属性可以在解析公式时将这些参数标记为数组模式。否则用户需要稍后通过[`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) 更新这些自定义函数以获得相同的结果。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCustomFunctionDefinitionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建自定义函数定义
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();
            
            // 使用自定义函数设置公式解析选项
            FormulaParseOptions options = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunction,
                Parse = true
            };

            // 设置示例数据
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);

            // 在公式中使用自定义函数
            string formula = "=MY_CUSTOM_FUNCTION(A1, B1)";
            worksheet.Cells["C1"].SetFormula(formula, options);

            // 计算工作簿以演示自定义函数处理
            workbook.CalculateFormula();

            // 保存结果
            workbook.Save("CustomFunctionDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


