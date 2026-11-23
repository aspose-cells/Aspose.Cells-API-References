---
title: "ShapePath.HeightPixel"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePath 属性。获取此路径的高度，单位为像素"
type: docs
url: /zh/net/aspose.cells.drawing/shapepath/heightpixel/
---
## ShapePath.HeightPixel property

获取此路径的高度，单位为像素。

```csharp
public int HeightPixel { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyHeightPixelDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 创建新的形状路径
                ShapePath shapePath = new ShapePath();

                // 创建一个简单的矩形路径
                shapePath.MoveTo(10, 10);
                shapePath.LineTo(100, 10);
                shapePath.LineTo(100, 50);
                shapePath.LineTo(10, 50);
                shapePath.Close();

                // 显示当前 HeightPixel 值
                Console.WriteLine("Initial HeightPixel value: " + shapePath.HeightPixel);

                // 设置新的高度值
                shapePath.HeightPixel = 200;
                Console.WriteLine("Updated HeightPixel value: " + shapePath.HeightPixel);

                // 将形状添加到工作表中
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                // 保存工作簿
                workbook.Save("HeightPixelDemo.xlsx");
                Console.WriteLine("HeightPixel property demonstrated successfully.");
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

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


