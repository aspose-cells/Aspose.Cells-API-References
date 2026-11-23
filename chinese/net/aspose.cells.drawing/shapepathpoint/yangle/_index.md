---
title: "ShapePathPoint.YAngle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePathPoint 属性。当对象是角度标记时，获取或设置第二个角度（单位：度）"
type: docs
url: /zh/net/aspose.cells.drawing/shapepathpoint/yangle/
---
## ShapePathPoint.YAngle property

当对象是角度标记时，获取或设置第二个角度（单位：度）。

```csharp
public int YAngle { get; set; }
```

### 备注

如果此角度是弧的摆动角度。该角度指定沿假设的圆路径在角度方向上弧线将延伸多远。弧线从起始角度的延伸始终沿顺时针方向围绕假设的圆。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyYAngleDemo
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

                // 添加带有角度标记的点（使用 XAngle 和 YAngle）
                ShapePathPoint point1 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point1.XAngle = 45;  // First angle in degrees
                point1.YAngle = 90;  // Second angle in degrees

                // 显示 YAngle 值
                Console.WriteLine($"Point 1 YAngle: {point1.YAngle} degrees");

                // 创建具有不同角度的另一个点
                ShapePathPoint point2 = pathPoints[pathPoints.Add(0, 0)]; // Get the added point
                point2.XAngle = 30;
                point2.YAngle = 60;

                // 显示 YAngle 值
                Console.WriteLine($"Point 2 YAngle: {point2.YAngle} degrees");

                // 创建形状路径并使用角度标记添加弧线
                ShapePath path = new ShapePath();
                path.ArcTo(point1.XAngle, point1.YAngle, 100, 100);

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
                workbook.Save("YAngleDemo.xlsx");
                Console.WriteLine("YAngle property demonstration completed successfully.");
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


