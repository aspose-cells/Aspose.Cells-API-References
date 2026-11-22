---
title: "GroupCharacterEquationNode.Position"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GroupCharacterEquationNode. تحدد هذه السمة موضع الحرف في الكائن"
type: docs
url: /ar/net/aspose.cells.drawing.equations/groupcharacterequationnode/position/
---
## GroupCharacterEquationNode.Position property

هذه السمة تحدد موضع الحرف في الكائن

```csharp
public EquationCharacterPositionType Position { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class GroupCharacterEquationNodePropertyPositionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة شكل معادلة إلى ورقة العمل الأولى
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // احصل على فقرة المعادلة وأضف عقدة حرف مجموعة
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            GroupCharacterEquationNode groupNode = (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            
            // تعيين خاصية الموضع (عرض توضيحي أساسي)
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // أضف النص الأساسي
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
            textNode.Text = "abc";

            // احفظ المصنف
            string outputPath = "GroupCharacterEquationDemo.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Equation with group character position set to Top has been created successfully.");
        }
    }
}
```

### انظر أيضًا

* enum [EquationCharacterPositionType](../../equationcharacterpositiontype/)
* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


