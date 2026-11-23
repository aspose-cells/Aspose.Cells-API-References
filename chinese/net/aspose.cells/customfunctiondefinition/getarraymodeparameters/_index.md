---
title: "CustomFunctionDefinition.GetArrayModeParameters"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CustomFunctionDefinition 方法。获取给定自定义函数参数中需要在数组模式下计算的索引"
type: docs
url: /zh/net/aspose.cells/customfunctiondefinition/getarraymodeparameters/
---
## CustomFunctionDefinition.GetArrayModeParameters method

获取给定自定义函数的参数在数组模式下需要计算的索引。

```csharp
public virtual int[] GetArrayModeParameters(string functionName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| functionName | String | 自定义函数的名称。 |

### 返回值

给定自定义函数中需要在数组模式下计算的参数索引。默认值为 null，表示没有参数需要在数组模式下计算。

### 备注

对于需要计算的表达式，以 A:A+B:B 为例：通常在数值模式下，它会根据当前单元格基准计算为单个值。但在数组模式下，A1+B1、A2+B2、A3+B3、... 的所有值都会被计算并用于计算。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFunctionDefinitionMethodGetArrayModeParametersWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 CustomFunctionDefinition 的实例
            CustomFunctionDefinition customFunction = new CustomFunctionDefinition();

            try
            {
                // 使用函数名称参数调用 GetArrayModeParameters
                string functionName = "SUM";
                int[] result = customFunction.GetArrayModeParameters(functionName);

                // 显示结果
                if (result != null)
                {
                    Console.WriteLine("Array mode parameters for function '{0}':", functionName);
                    foreach (int param in result)
                    {
                        Console.WriteLine(param);
                    }
                }
                else
                {
                    Console.WriteLine("No array mode parameters defined for function '{0}'", functionName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetArrayModeParameters method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("CustomFunctionDefinitionGetArrayModeParametersDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [CustomFunctionDefinition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


