---
title: "GroupCharacterEquationNode.VertJc"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GroupCharacterEquationNode. هذه السمة مع pos من groupChrPr تحدد التخطيط العمودي لكائن groupChr. حيث يحدد pos موضع حرف التجميع، ويحدد vertJc محاذاة الكائن بالنسبة إلى الخط الأساسي"
type: docs
url: /ar/net/aspose.cells.drawing.equations/groupcharacterequationnode/vertjc/
---
## GroupCharacterEquationNode.VertJc property

هذه السمة، مع الجمع مع pos في groupChrPr، تحدد التخطيط العمودي لكائن groupChr. حيث يحدد pos موضع حرف التجميع، ويحدد vertJc محاذاة الكائن بالنسبة للخط الأساسي.

```csharp
public EquationCharacterPositionType VertJc { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class GroupCharacterEquationNodePropertyVertJcDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل مربع نص لاحتواء المعادلة
            var shape = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 100, 100);
            
            // إنشاء كائن GroupCharacterEquationNode
            var equationNode = (GroupCharacterEquationNode)shape.GetEquationParagraph().AddChild(EquationNodeType.GroupChr);
            
            try
            {
                // تعيين الخصائص الأولية لعقدة المعادلة
                equationNode.GroupChr = "⏟";
                equationNode.ChrType = EquationCombiningCharacterType.BottomCurlyBracket;
                equationNode.Position = EquationCharacterPositionType.Bottom;
                
                // عرض خاصية VertJc (قراءة وكتابة)
                Console.WriteLine("Initial VertJc value: " + equationNode.VertJc);
                
                // تغيير قيمة VertJc
                equationNode.VertJc = EquationCharacterPositionType.Top;
                Console.WriteLine("Modified VertJc value: " + equationNode.VertJc);
                
                // احفظ المصنف
                workbook.Save("VertJcDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


