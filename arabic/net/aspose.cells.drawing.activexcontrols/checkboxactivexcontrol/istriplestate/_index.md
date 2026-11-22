---
title: "CheckBoxActiveXControl.IsTripleState"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CheckBoxActiveXControl. تشير إلى كيفية عرض التحكم المحدد للقيم الفارغة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/istriplestate/
---
## CheckBoxActiveXControl.IsTripleState property

يشير إلى كيفية عرض التحكم المحدد للقيم Null.

```csharp
public bool IsTripleState { get; set; }
```

### ملاحظات

| **الإعداد** | **الوصف** |
| --- | --- |
| True | سيتنقل العنصر عبر الحالات للقيم نعم، لا، و Null. يظهر العنصر باهتًا (رماديًا) عندما يتم ضبط خاصية Value على Null. |
| False | (افتراضي) سيتنقل العنصر عبر الحالات للقيم نعم ولا. تُعرض قيم Null كما لو كانت قيم لا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم CheckBox ActiveX مع جميع المعلمات المطلوبة
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 100, 30, 100, 30);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // تكوين الخصائص الأساسية
            checkBox.Caption = "Triple State Demo";
            
            // اعرض خاصية IsTripleState
            checkBox.IsTripleState = true; // Enable three states: Checked, Unchecked, and Indeterminate
            checkBox.Value = CheckValueType.Mixed; // Set to indeterminate state

            // احفظ المصنف
            workbook.Save("CheckBoxTripleStateDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


