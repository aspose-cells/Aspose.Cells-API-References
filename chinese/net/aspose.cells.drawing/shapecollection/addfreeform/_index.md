---
title: "ShapeCollection.AddFreeform"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ShapeCollection 方法。向工作表添加自由形状"
type: docs
url: /zh/net/aspose.cells.drawing/shapecollection/addfreeform/
---
## ShapeCollection.AddFreeform method

向工作表添加自由形状。

```csharp
public Shape AddFreeform(int topRow, int top, int leftColumn, int left, int height, int width, 
    ShapePath[] paths)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| topRow | Int32 | 左上行索引。 |
| 顶部 | Int32 | 表示自由形状相对于其左行的垂直偏移量，单位为像素。 |
| leftColumn | Int32 | 左上列索引。 |
| 左 | Int32 | 表示自由形状相对于其左列的水平偏移量，单位为像素。 |
| height | Int32 | 表示自由形状的高度，单位为像素。 |
| 宽度 | Int32 | 表示自由形状的宽度，单位为像素。 |
| paths | ShapePath[] | 表示用户定义的路径 |

### 返回值

一个自由形状。

### 备注

注意：参数中的宽度和高度可以是任意正整数值，而不是 ’paths' 指定的 ShapePath 数组的整体宽度和高度。它们之间是比例填充关系，即每个 ShapePath 对象会根据宽度和高度进行缩放。因此，当 ’paths' 中有多个对象时，需要合理设计每个 ShapePath 对象以满足预期。若只有一个 ShapePath 对象且没有其他要求，将该对象的宽度和高度作为参数值传入是一个不错的方案。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddFreeformWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // 创建自定义图形路径
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
            
            ShapePath shapePath1 = new ShapePath();
            shapePath1.MoveTo(0, 0);
            shapePath1.CubicBezierTo(48.24997f, 0.6844f,
                                96.5f, -7.148871f,
                                130, 11.517795f);
            shapePath1.CubicBezierTo(163.5f, 30.18446f,
                                182.24997f, 75.351f,
                                201, 120.517795f);
            shapePath1.MoveTo(150, 80);
            shapePath1.ArcTo(25, 25, 0, 270);
            
            // 向工作表添加自由形状
            shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath, shapePath1 });

            // 保存工作簿
            workbook.Save("AddFreeformDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Shape](../../shape/)
* class [ShapePath](../../shapepath/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


