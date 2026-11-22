---
title: "TextBoxActiveXControl.EnterFieldBehavior"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxActiveXControl. تحدد سلوك التحديد عند دخول العنصر. True تعني أن التحديد يبقى دون تغيير منذ آخر مرة كان فيها العنصر نشطًا. False تعني أنه سيتم تحديد كل النص داخل العنصر عند الدخول إليه."
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterfieldbehavior/
---
## TextBoxActiveXControl.EnterFieldBehavior property

يحدد سلوك الاختيار عند دخول العنصر. True يعني أن الاختيار يبقى دون تغيير منذ آخر مرة كان فيها العنصر نشطًا. False يعني أنه سيتم تحديد كل النص داخل العنصر عند الدخول إليه.

```csharp
public bool EnterFieldBehavior { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyEnterFieldBehaviorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم TextBox ActiveX مع المعلمات الصحيحة
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl textBox = 
                (Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl)shape.ActiveXControl;

            // اعرض خاصية EnterFieldBehavior
            Console.WriteLine("Initial EnterFieldBehavior: " + textBox.EnterFieldBehavior);
            
            // بدّل خاصية EnterFieldBehavior
            textBox.EnterFieldBehavior = !textBox.EnterFieldBehavior;
            Console.WriteLine("Toggled EnterFieldBehavior: " + textBox.EnterFieldBehavior);

            // اضبط EnterFieldBehavior إلى true صراحة
            textBox.EnterFieldBehavior = true;
            Console.WriteLine("Final EnterFieldBehavior: " + textBox.EnterFieldBehavior);
        }
    }
}
```

### انظر أيضًا

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


