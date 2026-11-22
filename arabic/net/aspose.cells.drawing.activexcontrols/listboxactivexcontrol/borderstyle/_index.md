---
title: "ListBoxActiveXControl.BorderStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBoxActiveXControl. يحصل على ويضبط نوع الحدود المستخدمة في التحكم"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/borderstyle/
---
## ListBoxActiveXControl.BorderStyle property

يحصل ويضبط نوع الإطار المستخدم من قبل العنصر.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ListBox ActiveX مع معلمات مصححة
            Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 
                1, 0, 1, 100, 150, 30); // Added height parameter
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // ضبط خاصية BorderStyle
            listBox.BorderStyle = ControlBorderType.None;

            // تحقق وأخرج نمط الحدود
            Console.WriteLine("BorderStyle: " + listBox.BorderStyle);

            workbook.Save("ListBoxBorderStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlBorderType](../../controlbordertype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


