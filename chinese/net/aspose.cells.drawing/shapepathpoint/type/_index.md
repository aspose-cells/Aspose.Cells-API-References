---
title: "ShapePathPoint.Type"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePathPoint 属性。指定当前对象的值类型"
type: docs
url: /zh/net/aspose.cells.drawing/shapepathpoint/type/
---
## ShapePathPoint.Type property

指定当前对象的值类型。

```csharp
public ShapePathPointValueType Type { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointPropertyTypeDemo
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

                // 添加一个位置坐标点
                int positionPointIndex = pathPoints.Add(100, 50);
                ShapePathPoint positionPoint = pathPoints[positionPointIndex];

                // 显示位置坐标的 Type 属性值
                Console.WriteLine($"Position Point Type: {positionPoint.Type}");
                Console.WriteLine($"Position Point Type is Position: {positionPoint.Type == ShapePathPointValueType.Position}");

                // 添加一个角度标记点
                int anglePointIndex = pathPoints.Add(0, 0);
                ShapePathPoint anglePoint = pathPoints[anglePointIndex];
                anglePoint.XAngle = 45;
                anglePoint.YAngle = 90;

                // 显示角度标记的 Type 属性值
                Console.WriteLine($"Angle Point Type: {anglePoint.Type}");
                Console.WriteLine($"Angle Point Type is Angle: {anglePoint.Type == ShapePathPointValueType.Angle}");

                // 创建形状路径并添加点
                ShapePath path = new ShapePath();
                path.MoveTo(positionPoint.XPixel, positionPoint.YPixel);
                path.ArcTo(anglePoint.XAngle, anglePoint.YAngle, 100, 100);
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
                workbook.Save("ShapePathPointTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
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

* enum [ShapePathPointValueType](../../shapepathpointvaluetype/)
* class [ShapePathPoint](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


