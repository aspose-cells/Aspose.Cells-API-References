---
title: "ShapePathPoint.YPixel"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePathPoint 属性。当对象是位置坐标时，获取或设置以像素为单位的 y 坐标"
type: docs
url: /zh/net/aspose.cells.drawing/shapepathpoint/ypixel/
---
## ShapePathPoint.YPixel property

当对象是位置坐标时，获取或设置以像素为单位的 y 坐标。

```csharp
public int YPixel { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYPixelDemo
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

                // 添加具有坐标的点
                pathPoints.Add(100, 50);

                // 访问第一个点并演示 YPixel 属性
                ShapePathPoint firstPoint = pathPoints[0];

                // 显示初始 YPixel 值（读取操作）
                Console.WriteLine($"Initial YPixel value: {firstPoint.YPixel}");

                // 为 YPixel 设置新值（因为它是可读写的）
                firstPoint.YPixel = 150;
                Console.WriteLine($"Updated YPixel value: {firstPoint.YPixel}");

                // 创建形状路径并使用该点
                ShapePath path = new ShapePath();
                path.MoveTo(firstPoint.XPixel, firstPoint.YPixel);

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
                workbook.Save("YPixelDemo.xlsx");
                Console.WriteLine("YPixel property demonstration completed successfully.");
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


