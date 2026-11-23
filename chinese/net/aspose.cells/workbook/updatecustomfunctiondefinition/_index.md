---
title: "Workbook.UpdateCustomFunctionDefinition"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Workbook 方法。更新自定义函数的定义"
type: docs
url: /zh/net/aspose.cells/workbook/updatecustomfunctiondefinition/
---
## Workbook.UpdateCustomFunctionDefinition method

更新自定义函数的定义。

```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 定义 | CustomFunctionDefinition | 针对用户特殊需求的自定义函数特殊定义。 |

### 备注

此方法可用于某些特殊场景。例如，如果用户需要某些自定义函数的参数以数组模式计算，则用户可以提供实现了[`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) 的自定义定义。公式数据更新后，在计算相应的自定义函数时，这些指定的参数将自动以数组模式计算。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUpdateCustomFunctionDefinitionWithCustomFunctionDDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // 添加示例数据
            sheet.Cells["B1"].PutValue(1);
            sheet.Cells["C1"].PutValue(2);
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["C2"].PutValue(8);

            // 创建自定义计算引擎
            var customEngine = new MyCustomCalculationEngine();
            
            // 使用自定义引擎设置计算选项
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };

            // 更新自定义函数定义
            wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());

            // 使用自定义函数设置公式
            sheet.Cells["A1"].Formula = "=MYFUNC(B:B+C:C)";
            
            // 计算公式
            wb.CalculateFormula(options);

            // 输出结果
            Console.WriteLine("Custom function result: " + sheet.Cells["A1"].Value);
        }
    }

    public class MyCustomFunctionDefinition : CustomFunctionDefinition
    {
        public override int[] GetArrayModeParameters(string functionName)
        {
            // 返回应在数组模式下处理的参数索引
            return new int[] { 0 }; // First parameter is array mode
        }
    }

    public class MyCustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYFUNC")
            {
                double sum = 0;
                var paramValue = data.GetParamValue(0);
                
                if (paramValue is object[,] arrayValue)
                {
                    foreach (var val in arrayValue)
                    {
                        if (val != null)
                        {
                            sum += Convert.ToDouble(val);
                        }
                    }
                }
                else
                {
                    sum += Convert.ToDouble(paramValue);
                }
                data.CalculatedValue = sum * 2; // Custom calculation logic
            }
        }
    }
}
```

### 另请参见

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


