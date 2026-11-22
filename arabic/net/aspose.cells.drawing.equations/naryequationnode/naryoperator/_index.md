---
title: "NaryEquationNode.NaryOperator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية NaryEquationNode. عامل nary. على سبيل المثال. يُنصح بشدة باستخدام السمة NaryOperatorType لتعيين عامل nary. استخدم هذا الإعداد الخاص إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف"
type: docs
url: /ar/net/aspose.cells.drawing.equations/naryequationnode/naryoperator/
---
## NaryEquationNode.NaryOperator property

عامل n-ary. على سبيل المثال "∑". يُنصح بشدة باستخدام الخاصية NaryOperatorType لتعيين عامل n-ary. استخدم هذا الإعداد إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف.

```csharp
public string NaryOperator { get; set; }
```

### ملاحظات

يجب ملاحظة أن هذه الخاصية تقبل حرفًا واحدًا فقط، وإذا تم تمرير عدة أحرف، يتم قبول الحرف الأول فقط.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryOperatorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل معادلة
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // الحصول على عقدة المعادلة
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // إنشاء عقدة عامل n-ary
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            
            // تعيين خصائص عامل n-ary
            naryNode.NaryOperator = "\u2211"; // Summation symbol
            naryNode.NaryGrow = true;

            // إضافة مؤشر سفلي (اختياري)
            EquationNode subscript = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subscriptText = (TextRunEquationNode)subscript.AddChild(EquationNodeType.Text);
            subscriptText.Text = "i=1";

            // إضافة مؤشر علوي (اختياري)
            EquationNode superscript = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode superscriptText = (TextRunEquationNode)superscript.AddChild(EquationNodeType.Text);
            superscriptText.Text = "n";

            // إضافة التعبير الأساسي
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";

            // احفظ المصنف
            workbook.Save("NaryOperatorDemo.xlsx");

            Console.WriteLine("Nary operator equation created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


