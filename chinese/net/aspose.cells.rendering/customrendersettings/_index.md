---
title: "类 CustomRenderSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Rendering.CustomRenderSettings 类。表示渲染期间的自定义设置"
type: docs
url: /zh/net/aspose.cells.rendering/customrendersettings/
---
## CustomRenderSettings class

表示渲染期间的自定义设置。

```csharp
public class CustomRenderSettings
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [CustomRenderSettings](customrendersettings/)() | 构造函数。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| virtual [GetCellBorderWidth](../../aspose.cells.rendering/customrendersettings/getcellborderwidth/)(CellBorderType) | 根据边框类型指定单元格边框宽度。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些示例数据
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "Border Width Test";

            try
            {
                // 使用默认构造函数创建 CustomRenderSettings 的实例
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // 演示使用不同边框类型的 GetCellBorderWidth 方法
                float thinWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // 显示结果
                Console.WriteLine($"Thin border width: {thinWidth}");
                Console.WriteLine($"Thick border width: {thickWidth}");
                Console.WriteLine($"Dashed border width: {dashedWidth}");

                // 保存工作簿
                workbook.Save("CustomRenderSettingsDemo.xlsx");
                Console.WriteLine("CustomRenderSettings demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CustomRenderSettings demonstration: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


