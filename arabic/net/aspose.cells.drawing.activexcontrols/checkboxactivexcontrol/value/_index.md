---
title: "CheckBoxActiveXControl.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CheckBoxActiveXControl. تشير إلى ما إذا كان العنصر محددًا أم لا"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/value/
---
## CheckBoxActiveXControl.Value property

يشير إلى ما إذا كان التحكم محددًا أم لا.

```csharp
public CheckValueType Value { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ActiveX من نوع CheckBox إلى ورقة العمل.
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 5, 0, 5, 0, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // ضبط الخصائص الأساسية بما في ذلك Value
            checkBox.Caption = "Check Me";
            checkBox.Value = CheckValueType.Checked; // Demonstrating Value property usage

            // احفظ المصنف
            workbook.Save("CheckBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


