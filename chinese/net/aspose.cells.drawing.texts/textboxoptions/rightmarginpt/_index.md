---
title: "TextBoxOptions.RightMarginPt"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextBoxOptions 属性。获取并设置以点为单位的右边距"
type: docs
url: /zh/net/aspose.cells.drawing.texts/textboxoptions/rightmarginpt/
---
## TextBoxOptions.RightMarginPt property

获取和设置以点为单位的右侧边距。

```csharp
public double RightMarginPt { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyRightMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加文本框
            int textBoxIndex = worksheet.TextBoxes.Add(1, 1, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "Sample Text";

            // 以点为单位设置右边距
            textBox.TextBoxOptions.RightMarginPt = 0.2d;

            // 保存工作簿
            workbook.Save("TextBoxRightMarginDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


