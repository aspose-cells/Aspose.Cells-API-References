---
title: "TextBox.GetEquationParagraph"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TextBox 方法。从 TextBox 对象的 TextBody 属性获取指定的数学段落。注意 1 当索引超出范围或未找到时返回 NULL。2 如果指定的索引位置不是数学段落，也返回 NULL。"
type: docs
url: /zh/net/aspose.cells.drawing/textbox/getequationparagraph/
---
## GetEquationParagraph(int) {#getequationparagraph_1}

从 TextBox 对象的 TextBody 属性获取指定的数学段落。注意：(1) 当索引超出范围或未找到时返回 NULL。(2) 如果指定的索引位置不是数学段落，也返回 NULL。

```csharp
public EquationNode GetEquationParagraph(int index)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | Int32 | 数学段落的位置索引，从 0 开始。 |

### 返回值

返回由索引指定的数学段落。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class TextBoxMethodGetEquationParagraphWithInt32Demo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加文本框
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // 向文本框添加一些公式内容
            textBox.Text = "\\sqrt{x^2 + y^2}";

            try
            {
                // 使用索引参数（Int32）调用 GetEquationParagraph
                EquationNode equationNode = textBox.GetEquationParagraph(0);

                if (equationNode != null)
                {
                    Console.WriteLine("Equation paragraph retrieved successfully.");
                    Console.WriteLine($"Equation type: {equationNode.EquationType}");
                    Console.WriteLine($"LaTeX representation: {equationNode.ToLaTeX()}");
                }
                else
                {
                    Console.WriteLine("No equation paragraph found at the specified index.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEquationParagraph method: {ex.Message}");
            }

            // 保存工作簿
            workbook.Save("TextBoxMethodGetEquationParagraphWithInt32Demo.xlsx");
        }
    }
}
```

### 另请参见

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## GetEquationParagraph() {#getequationparagraph}

从 TextBox 对象的 TextBody 属性获取第一个数学段落。

```csharp
public EquationNode GetEquationParagraph()
```

### 返回值

如果存在数学段落，返回第一个，否则返回 null。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class TextBoxMethodGetEquationParagraphDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int textBoxIndex = worksheet.TextBoxes.Add(5, 5, 200, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "$$\\sqrt{x^2+y^2}$$";
            
            EquationNode equationNode = textBox.GetEquationParagraph();
            
            if (equationNode != null)
            {
                Console.WriteLine("Equation LaTeX: " + equationNode.ToLaTeX());
                Console.WriteLine("Equation MathML: " + equationNode.ToMathML());
            }
            else
            {
                Console.WriteLine("No equation paragraph found");
            }
        }
    }
}
```

### 另请参见

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


