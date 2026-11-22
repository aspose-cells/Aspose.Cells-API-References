---
title: "NaryEquationNode.NaryGrow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "NaryEquationNode property. تحدد هذه السمة خاصية النمو لمعاملات nary على مستوى المستند. عندما تكون غير مفعلة، لا تنمو معاملات nary مثل التكاملات والمجاميع لتطابق حجم ارتفاع معاملها. عندما تكون مفعلة، ينمو معامل nary عموديًا ليتطابق مع ارتفاع معاملها."
type: docs
url: /ar/net/aspose.cells.drawing.equations/naryequationnode/narygrow/
---
## NaryEquationNode.NaryGrow property

تحدد هذه الخاصية خاصية النمو لعوامل n-ary على مستوى المستند. عندما تكون معطلة، لا تنمو عوامل n-ary مثل التكاملات والمجاميع لتطابق حجم ارتفاع المعامل الخاص بها. عندما تكون مفعلة، ينمو عامل n-ary عموديًا ليتطابق مع ارتفاع معاملاته.

```csharp
public bool NaryGrow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class NaryEquationNodePropertyNaryGrowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل معادلة
            TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);
            
            // الحصول على عقدة المعادلة
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            
            // إنشاء عقدة معامل nary مع تعيين خاصية NaryGrow إلى true
            NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);
            naryNode.NaryOperator = "∑";
            naryNode.NaryGrow = true; // This is the key property we're demonstrating
            
            // إضافة مؤشر سفلي (اختياري)
            EquationNode sub = naryNode.AddChild(EquationNodeType.Subscript);
            TextRunEquationNode subText = (TextRunEquationNode)sub.AddChild(EquationNodeType.Text);
            subText.Text = "i=1";
            
            // إضافة مؤشر علوي (اختياري)
            EquationNode sup = naryNode.AddChild(EquationNodeType.Superscript);
            TextRunEquationNode supText = (TextRunEquationNode)sup.AddChild(EquationNodeType.Text);
            supText.Text = "n";
            
            // إضافة قاعدة (مطلوب)
            EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode baseText = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            baseText.Text = "x_i";
            
            // احفظ المصنف
            workbook.Save("NaryGrowDemo.xlsx");
            
            Console.WriteLine("Equation with NaryGrow property created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


