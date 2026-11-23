---
title: "Shape.LineFormat"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Shape 属性。返回一个包含指定形状线条格式属性的 MsoLineFormat 对象"
type: docs
url: /zh/net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

返回一个包含指定形状线条格式属性的 MsoLineFormat 对象。

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### 备注

注意：此成员现已过时。请改用 Shape.Line 属性。该属性将在自 2016 年 7 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineFormatDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 在第一个工作表中添加一个矩形形状
            Worksheet worksheet = workbook.Worksheets[0];
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(3, 0, 2, 0, 70, 130);
            
            // 设置形状属性
            rectangle.Placement = PlacementType.FreeFloating;
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            
            // 演示 LineFormat 的用法
            rectangle.LineFormat.Weight = 3; // Set line weight
            rectangle.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            rectangle.Line.SolidFill.Color = System.Drawing.Color.DarkBlue; // Correct way to set line color
            
            // 保存工作簿
            workbook.Save("ShapeLineFormatDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


