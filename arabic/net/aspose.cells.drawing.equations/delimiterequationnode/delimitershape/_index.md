---
title: "DelimiterEquationNode.DelimiterShape"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DelimiterEquationNode. تحدد شكل الفواصل في كائن الفاصل"
type: docs
url: /ar/net/aspose.cells.drawing.equations/delimiterequationnode/delimitershape/
---
## DelimiterEquationNode.DelimiterShape property

يحدد شكل الفواصل في كائن الفاصل.

```csharp
public EquationDelimiterShapeType DelimiterShape { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyDelimiterShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // الحصول على عقدة المعادلة
            var mathNode = textBox.GetEquationParagraph().GetChild(0);

            // إنشاء عقدة فاصل بشكل مخصص
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";

            // إضافة محتوى داخل الفاصل
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Content";

            // احفظ المصنف
            workbook.Save("DelimiterShapeDemo.xlsx");

            Console.WriteLine("Workbook saved with delimiter equation demonstrating DelimiterShape property.");
        }
    }
}
```

### انظر أيضًا

* enum [EquationDelimiterShapeType](../../equationdelimitershapetype/)
* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


