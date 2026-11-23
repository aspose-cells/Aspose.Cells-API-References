---
title: "Shape.GetRichFormattings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Shape 方法。返回所有表示文本中字符范围的 Characters 对象"
type: docs
url: /zh/net/aspose.cells.drawing/shape/getrichformattings/
---
## Shape.GetRichFormattings method

返回所有表示文本中字符范围的 Characters 对象。

```csharp
public FontSetting[] GetRichFormattings()
```

### 返回值

所有 Characters 对象

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加带有富文本的形状（针对 AddRectangle 的正确参数计数）
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);
            shape.Text = "This is bold and this is italic";
            
            // 格式化文本的部分
            shape.Characters(0, 4).Font.IsBold = true;
            shape.Characters(13, 6).Font.IsItalic = true;

            // 获取富文本格式
            FontSetting[] formattings = shape.GetRichFormattings();

            // 显示格式信息
            Console.WriteLine("Rich text formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"Text segment: '{shape.Text.Substring(setting.StartIndex, setting.Length)}'");
                Console.WriteLine($"Start index: {setting.StartIndex}");
                Console.WriteLine($"Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}");
                Console.WriteLine($"Italic: {setting.Font.IsItalic}");
                Console.WriteLine();
            }
        }
    }
}
```

### 另请参见

* class [FontSetting](../../../aspose.cells/fontsetting/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


