---
title: "AccentEquationNode.AccentCharacter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AccentEquationNode. يحدد هذا السمة نوع العلامة الصوتية المركبة المرفقة بقاعدة وظيفة التشكيل. الحرف الصوتي الافتراضي هو U0302. يُنصح بشدة باستخدام السمة AccentType لتعيين الحرف الصوتي. استخدم إعداد هذه الخاصية إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف"
type: docs
url: /ar/net/aspose.cells.drawing.equations/accentequationnode/accentcharacter/
---
## AccentEquationNode.AccentCharacter property

تحدد هذه الخاصية نوع علامة التشكيل المركبة المرفقة بقاعدة دالة اللهجة. الحرف الافتراضي لللهجة هو U+0302. يُنصح بشدة باستخدام الخاصية AccentType لتعيين حرف اللهجة. استخدم إعداد هذه الخاصية إذا لم تتمكن من العثور على الحرف الذي تحتاجه في نوع معروف.

```csharp
public string AccentCharacter { get; set; }
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
    public class AccentEquationNodePropertyAccentCharacterDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة شكل معادلة إلى ورقة العمل الأولى
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // احصل على عقدة المعادلة وأضف عقدة تشكيل
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            
            // حدد الحرف الصوتي (القبّة في هذه الحالة)
            accentNode.AccentCharacter = "\u0302";

            // أضف النص الأساسي للتشكيل
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "x";

            // احفظ المصنف
            workbook.Save("AccentEquationDemo.xlsx");

            // تحقق من الملف المحفوظ عن طريق تحميله مرة أخرى
            Workbook loadedWorkbook = new Workbook("AccentEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            AccentEquationNode loadedAccentNode = (AccentEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            // أخرج الحرف الصوتي لتوضيح الخاصية
            Console.WriteLine("Accent Character: " + loadedAccentNode.AccentCharacter);
        }
    }
}
```

### انظر أيضًا

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


