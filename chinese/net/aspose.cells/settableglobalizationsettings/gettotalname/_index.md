---
title: "SettableGlobalizationSettings.GetTotalName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。获取特定函数的总计名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/gettotalname/
---
## SettableGlobalizationSettings.GetTotalName method

获取特定函数的总计名称。

```csharp
public override string GetTotalName(ConsolidationFunction functionType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| functionType | ConsolidationFunction | 函数类型。 |

### 返回值

函数的总计名称。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 SettableGlobalizationSettings 的实例
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // 使用 ConsolidationFunction.Sum 调用 GetTotalName
                string totalName = globalizationSettings.GetTotalName(ConsolidationFunction.Sum);
                
                // 显示结果
                Console.WriteLine($"Total name for Sum function: {totalName}");

                // 添加数据以演示效果（尽管 GetTotalName 不会修改电子表格）
                worksheet.Cells["A1"].PutValue("Values");
                worksheet.Cells["A2"].PutValue(10);
                worksheet.Cells["A3"].PutValue(20);
                worksheet.Cells["A4"].PutValue(30);
                worksheet.Cells["B1"].PutValue("Total");
                worksheet.Cells["B4"].Formula = "=SUM(A2:A4)";
                
                // 计算公式
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTotalName method: {ex.Message}");
            }
            
            // 保存工作簿
            workbook.Save("SettableGlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


