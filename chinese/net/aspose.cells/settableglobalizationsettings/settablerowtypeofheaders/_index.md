---
title: "SettableGlobalizationSettings.SetTableRowTypeOfHeaders"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableGlobalizationSettings 方法。设置由表头组成的表行的类型名称"
type: docs
url: /zh/net/aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/
---
## SettableGlobalizationSettings.SetTableRowTypeOfHeaders method

设置由表头组成的表行的类型名称。

```csharp
public void SetTableRowTypeOfHeaders(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfHeadersWithStringDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建一个表并添加一些数据
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");
            
            // 创建 ListObject（表）
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // 创建 SettableGlobalizationSettings 实例
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // 使用自定义表头类型名称调用 SetTableRowTypeOfHeaders
                settings.SetTableRowTypeOfHeaders("CustomHeaders");

                // 将设置应用于工作簿
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table header type name set to: CustomHeaders");
                Console.WriteLine("In formulas, '#CustomHeaders' will now represent the table header");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfHeaders method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("SetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


