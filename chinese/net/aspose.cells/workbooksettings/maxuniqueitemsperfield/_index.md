---
title: "WorkbookSettings.MaxUniqueItemsPerField"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorkbookSettings 属性。获取和设置每个字段唯一项的限制"
type: docs
url: /zh/net/aspose.cells/workbooksettings/maxuniqueitemsperfield/
---
## WorkbookSettings.MaxUniqueItemsPerField property

获取和设置每个字段唯一项的限制

```csharp
public int MaxUniqueItemsPerField { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookSettingsPropertyMaxUniqueItemsPerFieldDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问 WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            try
            {
                // 显示当前 MaxUniqueItemsPerField 值
                Console.WriteLine("Current MaxUniqueItemsPerField value: " + settings.MaxUniqueItemsPerField);

                // 演示为 MaxUniqueItemsPerField 设置新值
                settings.MaxUniqueItemsPerField = 1000;
                Console.WriteLine("After setting to 1000: " + settings.MaxUniqueItemsPerField);

                // 设置另一个值以展示其可变性
                settings.MaxUniqueItemsPerField = 5000;
                Console.WriteLine("After setting to 5000: " + settings.MaxUniqueItemsPerField);

                // 添加一些示例数据以使示例更有意义
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Orange");

                // 保存工作簿
                workbook.Save("MaxUniqueItemsPerFieldDemo.xlsx");
                Console.WriteLine("Workbook saved with MaxUniqueItemsPerField settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


