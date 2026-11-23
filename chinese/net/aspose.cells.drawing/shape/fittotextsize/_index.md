---
title: "GradientFill.SetPresetThemeGradient"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Shape 方法。重新计算适合显示全部文本内容的文本区域"
type: docs
url: /zh/net/aspose.cells.drawing/shape/fittotextsize/
---
## Shape.FitToTextSize method

重新计算适合显示全部文本内容的文本区域。

```csharp
public void FitToTextSize()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeMethodFitToTextSizeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加文本框形状
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 100);
            textBox.Text = "This is a sample text that will demonstrate the FitToTextSize method functionality.";

            try
            {
                // 显示原始尺寸
                Console.WriteLine($"Original Width: {textBox.Width}, Height: {textBox.Height}");

                // 调用 FitToTextSize 方法
                textBox.FitToTextSize();

                // 显示调整后的尺寸
                Console.WriteLine($"Adjusted Width: {textBox.Width}, Height: {textBox.Height}");
                Console.WriteLine("FitToTextSize method executed successfully");

                // 添加更多文本以展示效果
                textBox.Text += " Adding more text to show how the shape adjusts to fit the content.";
                textBox.FitToTextSize();
                Console.WriteLine($"Final Width: {textBox.Width}, Height: {textBox.Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FitToTextSize method: {ex.Message}");
            }

            // 保存结果
            workbook.Save("ShapeMethodFitToTextSizeDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


