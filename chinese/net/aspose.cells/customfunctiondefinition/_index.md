---
title: "类 CustomFunctionDefinition"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.CustomFunctionDefinition 类。使用用户自定义引擎进行计算的自定义函数定义"
type: docs
url: /zh/net/aspose.cells/customfunctiondefinition/
---
## CustomFunctionDefinition class

使用用户自定义引擎进行计算的自定义函数定义。

```csharp
public class CustomFunctionDefinition
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [CustomFunctionDefinition](customfunctiondefinition/)() | 默认构造函数。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| virtual [GetArrayModeParameters](../../aspose.cells/customfunctiondefinition/getarraymodeparameters/)(string) | 获取给定自定义函数的参数在数组模式下需要计算的索引。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionDemo
    {
        public static void CustomFunctionDefinitionExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 创建一个新的 CustomFunctionDefinition 实例
            CustomFunctionDefinition customFunctionDefinition = new CustomFunctionDefinition();

            // 创建一个新的 FormulaParseOptions 实例并设置 CustomFunctionDefinition
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunctionDefinition
            };

            // 向工作簿添加工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 定义自定义公式
            string customFormula = "=MY_CUSTOM_FUNCTION(A1, B1)";

            // 使用 FormulaParseOptions 解析自定义公式
            worksheet.Cells["C1"].Formula = customFormula;
            worksheet.Cells["C1"].SetFormula(customFormula, formulaParseOptions);

            // 保存工作簿
            workbook.Save("CustomFunctionDefinitionExample.xlsx");
            workbook.Save("CustomFunctionDefinitionExample.pdf");
            return;
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


