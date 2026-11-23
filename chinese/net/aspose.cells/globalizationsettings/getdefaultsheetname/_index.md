---
title: "GlobalizationSettings.GetDefaultSheetName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GlobalizationSettings 方法。获取自动添加工作表时的默认工作表名称。默认是 Sheet"
type: docs
url: /zh/net/aspose.cells/globalizationsettings/getdefaultsheetname/
---
## GlobalizationSettings.GetDefaultSheetName method

获取自动添加工作表时的默认工作表名称。默认是 "Sheet"。

```csharp
public virtual string GetDefaultSheetName()
```

### 返回值

自动添加工作表时的默认工作表名称

### 备注

自动添加的（例如通过 [`Add`](../../worksheetcollection/add/)）工作表的名称将是指定名称加上序号。例如，德国用户可能希望工作表名称为 "Tabellenblatt2" 而不是 "Sheet2"。此时用户可以实现此方法返回 "Tabellenblatt"。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetDefaultSheetNameDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 设置自定义全局化设置
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // 从自定义全局化设置获取默认工作表名称
                string defaultSheetName = workbook.Settings.GlobalizationSettings.GetDefaultSheetName();
                Console.WriteLine($"Default sheet name retrieved: {defaultSheetName}");

                // 添加一个新工作表，以演示基于自定义默认值的命名
                int sheetIndex = workbook.Worksheets.Add();
                Worksheet newWorksheet = workbook.Worksheets[sheetIndex];
                Console.WriteLine($"New worksheet name after method call: {newWorksheet.Name}");

                Console.WriteLine("GetDefaultSheetName method demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDefaultSheetName method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("MethodGetDefaultSheetNameDemo.xlsx");
        }
    }

    // 自定义全局化设置实现
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDefaultSheetName()
        {
            return "CustomSheet"; // Custom default sheet name
        }
    }
}
```

### 另请参见

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


