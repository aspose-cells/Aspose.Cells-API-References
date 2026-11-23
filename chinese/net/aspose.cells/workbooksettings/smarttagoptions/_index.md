---
title: "WorkbookSettings.SmartTagOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "WorkbookSettings 属性。获取智能标签的选项"
type: docs
url: /zh/net/aspose.cells/workbooksettings/smarttagoptions/
---
## WorkbookSettings.SmartTagOptions property

获取智能标签的选项。

```csharp
public SmartTagOptions SmartTagOptions { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySmartTagOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // 创建一个新的工作簿
                Workbook workbook = new Workbook();

                // 访问工作簿设置
                WorkbookSettings settings = workbook.Settings;

                // 读取 SmartTagOptions 属性
                var smartTagOptions = settings.SmartTagOptions;

                // 显示关于 SmartTagOptions 实例的信息
                Console.WriteLine("SmartTagOptions instance type: " + smartTagOptions.GetType().FullName);

                // 可选地，您可以通过 ToString() 检查默认状态
                Console.WriteLine("SmartTagOptions details: " + smartTagOptions.ToString());

                // 保存工作簿（文件将包含默认设置）
                workbook.Save("SmartTagOptionsDemo.xlsx");
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

* class [SmartTagOptions](../../../aspose.cells.markup/smarttagoptions/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


