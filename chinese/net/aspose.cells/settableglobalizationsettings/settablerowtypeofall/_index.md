---
title: "SettableGlobalizationSettings.SetTableRowTypeOfAll"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。设置引用表中由所有行组成的表行的类型名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/settablerowtypeofall/
---
## SettableGlobalizationSettings.SetTableRowTypeOfAll method

设置由引用表中的所有行组成的表行的类型名称。

```csharp
public void SetTableRowTypeOfAll(string name)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | String | 表行的类型名称 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfAllWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为表创建示例数据
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);

            // 创建表
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // 使用自定义名称调用 SetTableRowTypeOfAll
                settings.SetTableRowTypeOfAll("CompleteTable");

                // 将设置应用于工作簿
                workbook.Settings.GlobalizationSettings = settings;

                // 通过获取返回值来验证设置
                string rowType = settings.GetTableRowTypeOfAll();
                Console.WriteLine($"Table row type for all rows set to: {rowType}");

                // 添加一个使用自定义名称引用所有行的公式
                cells["C2"].Formula = "=SUM(#CompleteTable[Price])";
                Console.WriteLine($"Formula using custom row type: {cells["C2"].Formula}");

                // 计算公式
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result: {cells["C2"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfAll method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("MethodSetTableRowTypeOfAllWithStringDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


