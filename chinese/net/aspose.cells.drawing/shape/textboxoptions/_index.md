---
title: "Shape.TextBoxOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Shape 属性。获取形状中的文本信息"
type: docs
url: /zh/net/aspose.cells.drawing/shape/textboxoptions/
---
## Shape.TextBoxOptions property

获取形状中的文本信息

```csharp
public TextBoxOptions TextBoxOptions { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;

    public class ShapePropertyTextBoxOptionsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加文本框形状
            int textBoxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "This is a sample text box to demonstrate TextBoxOptions properties.";

            // 显示当前 TextBoxOptions 属性
            TextBoxOptions textBoxOptions = textBox.TextBoxOptions;
            Console.WriteLine("Current TextBoxOptions:");
            Console.WriteLine("Vertical Alignment: " + textBoxOptions.ShapeTextVerticalAlignment);
            Console.WriteLine("Resize To Fit Text: " + textBoxOptions.ResizeToFitText);
            Console.WriteLine("Text Direction: " + textBoxOptions.ShapeTextDirection);
            Console.WriteLine("Left Margin: " + textBoxOptions.LeftMarginPt + " pt");
            Console.WriteLine("Right Margin: " + textBoxOptions.RightMarginPt + " pt");

            // 修改 TextBoxOptions 属性
            textBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Middle;
            textBoxOptions.ResizeToFitText = true;
            textBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;
            textBoxOptions.LeftMarginPt = 10;
            textBoxOptions.RightMarginPt = 10;
            textBoxOptions.TopMarginPt = 5;
            textBoxOptions.BottomMarginPt = 5;

            // 保存工作簿
            workbook.Save("TextBoxOptionsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [TextBoxOptions](../../../aspose.cells.drawing.texts/textboxoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


