---
title: "ShapePath.CubicBezierTo"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapePath 方法。向当前图形追加一个三次贝塞尔曲线。起始点是当前图形的结束点。单位 像素"
type: docs
url: /zh/net/aspose.cells.drawing/shapepath/cubicbezierto/
---
## ShapePath.CubicBezierTo method

向当前图形追加一个三次贝塞尔曲线。起始点是当前图形的结束点。单位：像素。

```csharp
public void CubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, 
    float endY)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ctrX1 | Single | 曲线第一个控制点的 x 坐标（单位：像素）。 |
| ctrY1 | Single | 曲线第一个控制点的 y 坐标（单位：像素）。 |
| ctrX2 | Single | 曲线第二个控制点的 x 坐标（单位：像素）。 |
| ctrY2 | Single | 曲线第二个控制点的 y 坐标（单位：像素）。 |
| endX | Single | 曲线终点的 x 坐标（单位：像素）。 |
| endY | Single | 曲线终点的 y 坐标（单位：像素）。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCubicBezierToWithSingleSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

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


            //添加自由形状
            worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath1 });

            // 保存结果
            workbook.Save("ShapePathMethodCubicBezierToDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


