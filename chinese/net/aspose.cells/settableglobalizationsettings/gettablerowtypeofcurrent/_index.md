---
title: "SettableGlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。获取由引用表的当前行组成的表行的类型名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/gettablerowtypeofcurrent/
---
## SettableGlobalizationSettings.GetTableRowTypeOfCurrent method

获取由引用表中的当前行组成的表行的类型名称。

```csharp
public override string GetTableRowTypeOfCurrent()
```

### 返回值

表行的类型名称

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建表
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            table.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // 创建自定义全局化设置
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            settings.SetTableRowTypeOfCurrent("CurrentRow");

            // 将设置应用于工作簿
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // 获取当前行的类型名称
                string currentRowType = settings.GetTableRowTypeOfCurrent();
                Console.WriteLine("Current row type name: " + currentRowType);

                // 添加引用当前行的公式
                cells["C2"].Formula = "=SUM(#CurrentRow)";
                Console.WriteLine("Formula set to: " + cells["C2"].Formula);

                // 计算公式
                workbook.CalculateFormula();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


