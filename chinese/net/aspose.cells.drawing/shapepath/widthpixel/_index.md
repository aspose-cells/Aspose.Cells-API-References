---
title: "ShapePath.WidthPixel"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePath 属性。获取此路径的宽度，单位为像素"
type: docs
url: /zh/net/aspose.cells.drawing/shapepath/widthpixel/
---
## ShapePath.WidthPixel property

获取此路径的宽度，单位为像素。

```csharp
public int WidthPixel { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyWidthPixelDemo
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

                // 显示初始 WidthPixel 值
                Console.WriteLine("Initial WidthPixel value: " + shapePath.WidthPixel);

                // 设置新的宽度值
                shapePath.WidthPixel = 300;
                Console.WriteLine("Updated WidthPixel value: " + shapePath.WidthPixel);

                // 将形状添加到工作表中
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, shapePath.WidthPixel, 200, new ShapePath[] { shapePath });

                // 保存工作簿
                workbook.Save("WidthPixelDemo.xlsx");
                Console.WriteLine("WidthPixel property demonstrated successfully.");
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


