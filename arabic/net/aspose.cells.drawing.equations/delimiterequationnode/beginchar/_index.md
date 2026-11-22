---
title: "DelimiterEquationNode.BeginChar"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DelimiterEquationNode. حرف بداية الفاصل"
type: docs
url: /ar/net/aspose.cells.drawing.equations/delimiterequationnode/beginchar/
---
## DelimiterEquationNode.BeginChar property

حرف بداية الفاصل.

```csharp
public string BeginChar { get; set; }
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
    public class DelimiterEquationNodePropertyBeginCharDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة معادلة إلى ورقة العمل الأولى
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);
            
            // الحصول على عقدة الجذر للمعادلة
            var mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // إضافة عقدة فاصل مع أحرف بداية/نهاية مخصصة
            var delimiterNode = mathNode.AddChild(EquationNodeType.Delimiter) as DelimiterEquationNode;
            delimiterNode.BeginChar = "#";
            delimiterNode.EndChar = "*";
            delimiterNode.DelimiterShape = EquationDelimiterShapeType.Match;
            
            // إضافة محتوى داخل الفاصل
            var baseNode = delimiterNode.AddChild(EquationNodeType.Base);
            var textNode = baseNode.AddChild(EquationNodeType.Text) as TextRunEquationNode;
            textNode.Text = "Sample Content";
            
            // احفظ المصنف
            string outputPath = "DelimiterEquationDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Workbook saved with custom delimiter equation. BeginChar: " + delimiterNode.BeginChar);
        }
    }
}
```

### انظر أيضًا

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


