---
title: "TextBoxOptions.WrapTextInShape"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextBoxOptions 属性。指定形状内的文本换行。False  不会对文本主体进行换行。True  将对文本主体进行换行"
type: docs
url: /zh/net/aspose.cells.drawing.texts/textboxoptions/wraptextinshape/
---
## TextBoxOptions.WrapTextInShape property

指定形状内的文本换行。False - 文本主体不会换行。True - 文本主体会换行。

```csharp
public bool WrapTextInShape { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyWrapTextInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加一个具有正确参数的文本框形状
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // 设置将在形状内换行的文本
            textBox.Text = "This is a long text that should wrap within the text box shape boundaries when WrapTextInShape is enabled.";

            // 启用形状内的文本换行
            textBox.TextBoxOptions.WrapTextInShape = true;

            // 保存工作簿
            workbook.Save("TextBoxWrapTextDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


