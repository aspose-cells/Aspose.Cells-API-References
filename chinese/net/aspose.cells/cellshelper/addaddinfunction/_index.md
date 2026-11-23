---
title: "CellsHelper.AddAddInFunction"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CellsHelper 方法。添加外接函数"
type: docs
url: /zh/net/aspose.cells/cellshelper/addaddinfunction/
---
## CellsHelper.AddAddInFunction method

添加外接函数。

```csharp
[Obsolete("Use WorksheetCollection.RegisterAddInFunction() methods instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static void AddAddInFunction(string function, int minCountOfParameters, 
    int maxCountOfParameters, ParameterType[] paramersType, ParameterType functionValueType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 函数 | String | 函数名称。 |
| minCountOfParameters | Int32 | 此函数所需的最小参数数量 |
| maxCountOfParameters | Int32 | 此函数允许的最大参数数量。 |
| paramersType | ParameterType[] | 函数的预期参数类型 |
| functionValueType | ParameterType | 函数的值类型。 |

### 备注

注意：此成员现已过时。请改用 WorksheetCollection.RegisterAddInFunction() 方法。该方法将在自 2022 年 1 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodAddAddInFunctionWithStringInt32Int32ParameterTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 为 AddAddInFunction 定义参数
                string functionName = "CUSTOMFUNCTION";
                int minParams = 2;
                int maxParams = 4;
                ParameterType[] paramTypes = new ParameterType[] { ParameterType.Value, ParameterType.Reference };
                ParameterType returnType = ParameterType.Value;

                // 调用 AddAddInFunction 方法
                CellsHelper.AddAddInFunction(functionName, minParams, maxParams, paramTypes, returnType);

                // 在单元格中使用自定义函数
                worksheet.Cells["A1"].Formula = "=CUSTOMFUNCTION(5,B2)";
                worksheet.Cells["B2"].Value = 10;

                // 计算公式
                workbook.CalculateFormula();

                Console.WriteLine("AddAddInFunction executed successfully. Custom function added and used in A1.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAddInFunction method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("AddAddInFunctionDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [ParameterType](../../parametertype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


