---
title: "GroupCharacterEquationNode.GroupChr"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GroupCharacterEquationNode. تحدد رمزًا افتراضيًا U23DF. يُنصح بشدة باستخدام السمة ChrType لتعيين حرف التشكيل. استخدم إعداد هذه الخاصية إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف"
type: docs
url: /ar/net/aspose.cells.drawing.equations/groupcharacterequationnode/groupchr/
---
## GroupCharacterEquationNode.GroupChr property

يحدد رمزًا (الافتراضي U+23DF). يُنصح بشدة باستخدام السمة ChrType لتعيين حرف التشكيل. استخدم إعداد الخاصية هذا إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف.

```csharp
public string GroupChr { get; set; }
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
    public class GroupCharacterEquationNodePropertyGroupChrDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة معادلة إلى ورقة العمل الأولى
            TextBox textBox = workbook.Worksheets[0].Shapes.AddTextBox(3, 0, 3, 0, 100, 200);

            // الحصول على عقدة الجذر للمعادلة
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

            // إنشاء عقدة حرف مجموعة بسهم مزدوج إلى اليمين
            GroupCharacterEquationNode groupNode = 
                (GroupCharacterEquationNode)mathNode.AddChild(EquationNodeType.GroupChr);
            groupNode.Position = EquationCharacterPositionType.Top;
            groupNode.ChrType = EquationCombiningCharacterType.RightwardsDoubleArrow;

            // إضافة النص الأساسي إلى حرف المجموعة
            EquationNode baseNode = groupNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = 
                (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "abc";

            // عرض استخدام خاصية GroupChr
            Console.WriteLine("Group Character: " + groupNode.GroupChr); // Should output "⇒"

            // احفظ المصنف
            workbook.Save("GroupCharacterEquationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GroupCharacterEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


