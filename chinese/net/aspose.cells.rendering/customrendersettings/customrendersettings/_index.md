---
title: "CustomRenderSettings.CustomRenderSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CustomRenderSettings 构造函数。Ctor"
type: docs
url: /zh/net/aspose.cells.rendering/customrendersettings/customrendersettings/
---
## CustomRenderSettings constructor

构造函数。

```csharp
public CustomRenderSettings()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodSharpctorDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些上下文数据
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";

            try
            {
                // 使用构造函数创建 CustomRenderSettings 的实例
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // 显示构造函数调用成功的确认信息
                Console.WriteLine("CustomRenderSettings instance created successfully using #ctor");

                // 通过调用方法演示实例可正常工作
                float borderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                Console.WriteLine($"Default thin border width: {borderWidth}");

                // 保存工作簿
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomRenderSettings: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


