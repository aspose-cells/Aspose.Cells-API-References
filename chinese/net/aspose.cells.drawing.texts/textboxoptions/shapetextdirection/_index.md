---
title: "TextBoxOptions.ShapeTextDirection"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextBoxOptions 属性。获取或设置给定文本主体内的文本显示方向。它对应于 Excel 中的 Format Shape  Text Options  Text Box  Text direction。"
type: docs
url: /zh/net/aspose.cells.drawing.texts/textboxoptions/shapetextdirection/
---
## TextBoxOptions.ShapeTextDirection property

获取或设置给定文本主体内的文本显示方向。它对应 Excel 中的“格式形状 - 文本选项 - 文本框 - 文本方向”。

```csharp
public TextVerticalType ShapeTextDirection { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyShapeTextDirectionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加文本框形状
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // 将文本方向设置为垂直
            shape.TextBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;

            // 设置一些文本以演示方向
            shape.Text = "Vertical Text Example";

            // 保存工作簿
            workbook.Save("TextBoxTextDirectionDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [TextVerticalType](../../textverticaltype/)
* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


