---
title: "ShapePathPoint.XPixel"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePathPoint 属性。当对象是位置坐标时，获取或设置以像素为单位的 x 坐标"
type: docs
url: /zh/net/aspose.cells.drawing/shapepathpoint/xpixel/
---
## ShapePathPoint.XPixel property

当对象是位置坐标时，获取或设置以像素为单位的 x 坐标。

```csharp
public int XPixel { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXPixelDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 创建形状路径点集合
                ShapePathPointCollection pathPoints = new ShapePathPointCollection();

                // 添加带坐标的点
                pathPoints.Add(100, 50);
                pathPoints.Add(200, 100);

                // 访问第一个点并演示 XPixel 属性
                ShapePathPoint firstPoint = pathPoints[0];

                // 显示 XPixel 值（读取操作）
                Console.WriteLine($"Initial XPixel value: {firstPoint.XPixel}");

                // 为 XPixel 设置新值（因为它是可读写的）
                firstPoint.XPixel = 150;
                Console.WriteLine($"Updated XPixel value: {firstPoint.XPixel}");

                // 创建形状路径并添加这些点
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

                // 添加第二个点
                ShapePathPoint secondPoint = pathPoints[1];
                path.LineTo(secondPoint.XPixel, secondPoint.YPixel);
                path.Close();

                // 向工作表添加自由形状
                worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path });

                // 保存工作簿
                workbook.Save("XPixelDemo.xlsx");
                Console.WriteLine("XPixel property demonstration completed successfully.");
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

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


