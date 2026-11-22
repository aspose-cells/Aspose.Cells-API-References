---
title: "DelimiterEquationNode.EndChar"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DelimiterEquationNode. حرف انتهاء الفاصل"
type: docs
url: /ar/net/aspose.cells.drawing.equations/delimiterequationnode/endchar/
---
## DelimiterEquationNode.EndChar property

حرف نهاية الفاصل.

```csharp
public string EndChar { get; set; }
```

### ملاحظات

يجب ملاحظة أن هذه الخاصية تقبل حرفًا واحدًا فقط، وإذا تم تمرير عدة أحرف، يتم قبول الحرف الأول فقط.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyEndCharDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // الحصول على عقدة المعادلة
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // إنشاء عقدة فاصل مع حرف انتهاء مخصص
            var delimiterNode = (DelimiterEquationNode)mathNode.AddChild(EquationNodeType.Delimiter);
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]"; // Demonstrating EndChar property
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;

            // إضافة محتوى داخل الفاصل
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "Content";

            // حفظ والتحقق
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);

            // تحقق من الملف المحفوظ
            Workbook verifyWorkbook = new Workbook(outputPath);
            var verifyTextBox = (TextBox)verifyWorkbook.Worksheets[0].Shapes[0];
            var verifyNode = (DelimiterEquationNode)verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0);

            Console.WriteLine("BeginChar: " + verifyNode.BeginChar);
            Console.WriteLine("EndChar: " + verifyNode.EndChar); // Output the EndChar value
        }
    }
}
```

### انظر أيضًا

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


