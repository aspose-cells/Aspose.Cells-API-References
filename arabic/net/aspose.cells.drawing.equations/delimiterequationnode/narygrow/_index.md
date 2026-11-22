---
title: "DelimiterEquationNode.NaryGrow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DelimiterEquationNode. تحدد ما إذا كان الفاصل يجب أن يتوسع ويتقلص تلقائيًا مع ارتفاع الصيغة"
type: docs
url: /ar/net/aspose.cells.drawing.equations/delimiterequationnode/narygrow/
---
## DelimiterEquationNode.NaryGrow property

يحدد ما إذا كان الفاصل يجب أن يتوسع ويتقلص تلقائيًا مع ارتفاع الصيغة.

```csharp
public bool NaryGrow { get; set; }
```

### ملاحظات

تحدد هذه الخاصية خاصية النمو للفاصل على مستوى المستند. عندما تكون معطلة، لن يتوسع الفاصل لمطابقة حجم ارتفاع مكوّنه. عندما تكون مفعلة، ينمو الفاصل عموديًا لمطابقة ارتفاع مكوّنه.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DelimiterEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            var textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            var paragraph = textBox.GetEquationParagraph();
            var mathNode = paragraph.GetChild(0);
            
            // إنشاء عقدة فاصل باستخدام خاصية NaryGrow
            var delimiterNode = mathNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Delimiter) 
                as Aspose.Cells.Drawing.Equations.DelimiterEquationNode;
            delimiterNode.DelimiterShape = Aspose.Cells.Drawing.Equations.EquationDelimiterShapeType.Match;
            delimiterNode.NaryGrow = false; // Demonstrating NaryGrow property
            delimiterNode.BeginChar = "[";
            delimiterNode.EndChar = "]";
            delimiterNode.SeparatorChar = ",";

            // أضف العناصر الأساسية
            var baseNode1 = delimiterNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
            var textNode1 = baseNode1.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text) 
                as Aspose.Cells.Drawing.Equations.TextRunEquationNode;
            textNode1.Text = "x";

            var baseNode2 = delimiterNode.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Base);
            var textNode2 = baseNode2.AddChild(Aspose.Cells.Drawing.Equations.EquationNodeType.Text) 
                as Aspose.Cells.Drawing.Equations.TextRunEquationNode;
            textNode2.Text = "y";

            // حفظ والتحقق
            string outputFile = "DelimiterEquationNode_NaryGrow_Demo.xlsx";
            workbook.Save(outputFile);

            // تحقق من الملف المحفوظ
            Workbook verifyWorkbook = new Workbook(outputFile);
            var verifyTextBox = verifyWorkbook.Worksheets[0].Shapes[0] as Aspose.Cells.Drawing.TextBox;
            var verifyNode = verifyTextBox.GetEquationParagraph().GetChild(0).GetChild(0) 
                as Aspose.Cells.Drawing.Equations.DelimiterEquationNode;
            
            Console.WriteLine("NaryGrow value: " + verifyNode.NaryGrow); // Should output "False"
        }
    }
}
```

### انظر أيضًا

* class [DelimiterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


