---
title: "ImageOrPrintOptions.GridlineColor"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ImageOrPrintOptions 属性。获取或设置网格线颜色"
type: docs
url: /zh/net/aspose.cells.rendering/imageorprintoptions/gridlinecolor/
---
## ImageOrPrintOptions.GridlineColor property

获取或设置网格线颜色。

```csharp
public Color GridlineColor { get; set; }
```

### 备注

它将忽略源文件中的网格线颜色设置。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 放入一些示例数据，使工作表具有内容
            worksheet.Cells["A1"].PutValue("Demo for GridlineColor property");

            try
            {
                // 创建 ImageOrPrintOptions 的实例
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // 显示当前 GridlineColor 值（只读或读写）
                // 属性类型假定为 System.Drawing.Color
                Console.WriteLine("Current GridlineColor: " + options.GridlineColor);

                // 可选地将工作表渲染为图像，以查看默认网格线颜色的效果
                // （无需更改该值；我们仅演示用法。）
                SheetRender renderer = new SheetRender(worksheet, options);
                renderer.ToImage(0, "GridlineColorDemo.png");

                // 保存工作簿（可选）
                workbook.Save("GridlineColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during demo: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


