---
title: "TextBox.GetEquationParagraph"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TextBox. احصل على الفقرة الرياضية المحددة من خاصية TextBody لكائن TextBox. ملاحظة 1: تُعيد NULL عندما يكون الفهرس خارج النطاق أو غير موجود. 2: تُعيد أيضًا NULL إذا لم تكن الموضع المحدد فقرًا رياضيًا."
type: docs
url: /ar/net/aspose.cells.drawing/textbox/getequationparagraph/
---
## GetEquationParagraph(int) {#getequationparagraph_1}

احصل على الفقرة الرياضية المحددة من خاصية TextBody لكائن TextBox. ملاحظة: (1) تُعيد NULL عندما يكون الفهرس خارج النطاق أو غير موجود. (2) تُعيد NULL أيضًا إذا لم يكن موضع الفهرس المحدد فقرة رياضية.

```csharp
public EquationNode GetEquationParagraph(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس الموضع للفقرة الرياضية، يبدأ من 0. |

### قيمة الإرجاع

يرجع الفقرة الرياضية المحددة بواسطة الفهرس.

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مربع نص إلى ورقة العمل
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // أضف بعض محتوى المعادلة إلى مربع النص
            textBox.Text = "\\sqrt{x^2 + y^2}";

            try
            {
                // استدعِ GetEquationParagraph مع معامل الفهرس (Int32)
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

            // احفظ المصنف
            workbook.Save("TextBoxMethodGetEquationParagraphWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## GetEquationParagraph() {#getequationparagraph}

يحصل على الفقرة الرياضية الأولى من خاصية TextBody لكائن TextBox.

```csharp
public EquationNode GetEquationParagraph()
```

### قيمة الإرجاع

إذا كان هناك فقرة رياضية، يرجع الأولى، وإلا يرجع null.

### أمثلة

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

### انظر أيضًا

* class [EquationNode](../../../aspose.cells.drawing.equations/equationnode/)
* class [TextBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


