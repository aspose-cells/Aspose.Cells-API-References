---
title: "SettableGlobalizationSettings.SetGrandTotalName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。设置特定函数的总计名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/setgrandtotalname/
---
## SettableGlobalizationSettings.SetGrandTotalName method

设置特定函数的总计名称。

```csharp
public void SetGrandTotalName(ConsolidationFunction functionType, string name)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| functionType | ConsolidationFunction | 函数类型。 |
| 名称 | String | 函数的总计名称。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettableGlobalizationSettingsMethodSetGrandTotalNameWithConsolidationFunctionStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为数据透视表创建示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(75);

            // 创建数据透视表
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;

            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // 使用 ConsolidationFunction.Sum 调用 SetGrandTotalName 并提供自定义名称
                settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Grand Total");

                // 刷新数据透视表以应用更改
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Grand total name set to 'Custom Grand Total' for Sum function");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGrandTotalName method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("MethodSetGrandTotalNameDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


