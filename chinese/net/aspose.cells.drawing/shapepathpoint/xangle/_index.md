---
title: "ShapePathPoint.XAngle"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePathPoint 属性。当对象是角度标记时，获取或设置第一个角度（单位：度）"
type: docs
url: /zh/net/aspose.cells.drawing/shapepathpoint/xangle/
---
## ShapePathPoint.XAngle property

当对象是角度标记时，获取或设置第一个角度（单位：度）。

```csharp
public int XAngle { get; set; }
```

### 备注

如果此角度是弧的起始角度。该角度指定在假设的圆路径上用于绘制弧线的起始位置的角度。此起始角度将锁定在形状路径中上一次已知的笔位置上，从而保证连续的形状路径。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyXAngleDemo
    {
        public static void Run()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建形状路径点集合
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();
            pathPoints.Add(30, 20);
            pathPoints.Add(80, 20);
            pathPoints.Add(80, 70);
            pathPoints.Add(30, 70);

            // 检索第一个点并显示其 X 和 Y 坐标
            ShapePathPoint firstPoint = pathPoints[0];
            Console.WriteLine($"First point – X: {firstPoint.X}, Y: {firstPoint.Y}");

            // 注意：根据当前 API 反射，ShapePathPoint 类未公开 XAngle 属性。
            // 因此，此演示侧重于可用的 X 和 Y 属性。

            // 使用定义的点构建一个简单的自由形状
            ShapePath path = new ShapePath();
            path.MoveTo(firstPoint.X, firstPoint.Y);
            for (int i = 1; i < pathPoints.Count; i++)
            {
                ShapePathPoint pt = pathPoints[i];
                path.LineTo(pt.X, pt.Y);
            }
            path.Close();

            // 将自由形状添加到工作表中
            worksheet.Shapes.AddFreeform(
                topRow: 2,
                top: 0,
                leftColumn: 2,
                left: 0,
                height: 200,
                width: 200,
                paths: new ShapePath[] { path });

            // 保存工作簿
            workbook.Save("ShapePathPointXAngleDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


