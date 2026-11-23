---
title: "FillFormat.Type"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "FillFormat 属性。获取和设置填充类型"
type: docs
url: /zh/net/aspose.cells.drawing/fillformat/type/
---
## FillFormat.Type property

获取和设置填充类型。

```csharp
[Obsolete("Use FillFormat.FillType  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FillType Type { get; set; }
```

### 备注

注意：此成员现已过时。请改用 FillFormat.FillType 属性。此属性将在自 2016 年 7 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加矩形形状
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
            FillFormat fill = shape.Fill;

            // 显示当前 Type 值
            Console.WriteLine("Current Type value: " + fill.Type);

            // 将 Type 更改为 Gradient（此属性已过时，仅用于演示）
            fill.Type = FillType.Gradient;

            // 应用双色渐变效果
            fill.SetTwoColorGradient(Color.Blue, Color.Green, GradientStyleType.Horizontal, 1);

            // 保存已修改的工作簿
            workbook.Save("FillFormatTypeDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


