---
title: "ShapePath.ArcTo"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePath 方法。向当前图形追加一个椭圆弧。起始点是当前图形的结束点"
type: docs
url: /zh/net/aspose.cells.drawing/shapepath/arcto/
---
## ShapePath.ArcTo method

向当前图形追加椭圆弧。起始点是当前图形的结束点。

```csharp
public void ArcTo(float wR, float hR, float stAng, float swAng)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| wR | Single | 绘制弧线的椭圆矩形区域的半宽度（单位: Pixel）。 |
| hR | Single | 绘制弧线的椭圆矩形区域的半高度（单位: Pixel）。 |
| stAng | Single | 弧线的起始角度，以从 x 轴顺时针方向的度数测量（单位: Degree）。该角度指定在假想圆路径上用于绘制弧线的起始位置。此起始角度将锁定到形状路径中上一次已知的笔位置，从而保证形状路径的连续性。 |
| swAng | Single | 弧线的摆动角度。该角度指定弧线在假想圆路径上沿角度方向延伸的距离。延伸将始终从起始角度沿顺时针方向围绕假想圆进行。（单位: Degree） |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodArcToWithSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            //创建新的形状路径
            ShapePath shapePath = new ShapePath();
            shapePath.MoveTo(60, 45);
            shapePath.ArcTo(25, 25, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(60, 20);
            shapePath.LineTo(110, 70);
            shapePath.LineTo(125, 155.5f);
            shapePath.ArcTo(35.5f, 35.5f, 0, 270);
            shapePath.Close();

            shapePath.MoveTo(150, 45);
            shapePath.ArcTo(25, 25, 0, 270);

            //创建新的形状路径
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                        96.5f, -7.148871f,
                        130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                        182.24997f, 75.351f,
                        201, 120.517795f);
            shapePath1.MoveTo(150, 70);
            shapePath1.ArcTo(25, 25, 0, 270);

            Workbook workbook = new Workbook();

            //添加自由形状
            workbook.Worksheets[0].Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath, shapePath1 });

            // 保存结果
            workbook.Save("ShapePathMethodArcToDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


