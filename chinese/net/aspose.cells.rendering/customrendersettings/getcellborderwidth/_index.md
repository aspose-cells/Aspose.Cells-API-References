---
title: "CustomRenderSettings.GetCellBorderWidth"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "CustomRenderSettings 方法。根据边框类型指定单元格边框宽度"
type: docs
url: /zh/net/aspose.cells.rendering/customrendersettings/getcellborderwidth/
---
## CustomRenderSettings.GetCellBorderWidth method

根据边框类型指定单元格边框宽度。

```csharp
public virtual float GetCellBorderWidth(CellBorderType borderType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| borderType | CellBorderType | 单元格边框类型 |

### 返回值

单元格边框宽度

### 备注

任何负值将被忽略。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class CustomRenderSettingsMethodGetCellBorderWidthWithCellBorderTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一些上下文数据
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // 创建 CustomRenderSettings 的实例
                CustomRenderSettings renderSettings = new CustomRenderSettings();

                // 使用不同的边框类型调用 GetCellBorderWidth
                float thinBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thin);
                float thickBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Thick);
                float dashedBorderWidth = renderSettings.GetCellBorderWidth(CellBorderType.Dashed);

                // 显示结果
                Console.WriteLine($"Thin border width: {thinBorderWidth}");
                Console.WriteLine($"Thick border width: {thickBorderWidth}");
                Console.WriteLine($"Dashed border width: {dashedBorderWidth}");

                // 保存工作簿
                workbook.Save("GetCellBorderWidthDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [CellBorderType](../../../aspose.cells/cellbordertype/)
* class [CustomRenderSettings](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


