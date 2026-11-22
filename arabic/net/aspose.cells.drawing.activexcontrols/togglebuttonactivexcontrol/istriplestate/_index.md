---
title: "ToggleButtonActiveXControl.IsTripleState"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ToggleButtonActiveXControl. تشير إلى كيفية عرض العنصر المحدد للقيم Null"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/istriplestate/
---
## ToggleButtonActiveXControl.IsTripleState property

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

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyIsTripleStateDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر ToggleButton ActiveX control
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 0, 1, 0, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // اضبط خاصية IsTripleState إلى true
            toggleButton.IsTripleState = true;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // غيّر خاصية IsTripleState إلى false
            toggleButton.IsTripleState = false;
            Console.WriteLine("ToggleButton IsTripleState: " + toggleButton.IsTripleState);

            // احفظ المصنف
            workbook.Save("ToggleButtonIsTripleStateDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


