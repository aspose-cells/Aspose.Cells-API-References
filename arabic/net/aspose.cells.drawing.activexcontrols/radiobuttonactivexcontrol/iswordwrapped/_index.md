---
title: "RadioButtonActiveXControl.IsWordWrapped"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RadioButtonActiveXControl. تشير إلى ما إذا كان محتوى العنصر يلتف تلقائيًا في نهاية السطر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/iswordwrapped/
---
## RadioButtonActiveXControl.IsWordWrapped property

يشير إلى ما إذا كان محتوى العنصر يلتف تلقائيًا في نهاية السطر.

```csharp
public bool IsWordWrapped { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر RadioButton ActiveX control
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton,
                1, 1, 100, 50, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl radioButton = 
                (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape.ActiveXControl;

            // إظهار خاصية IsWordWrapped
            Console.WriteLine("Initial IsWordWrapped value: " + radioButton.IsWordWrapped);
            
            radioButton.IsWordWrapped = true;
            Console.WriteLine("After setting IsWordWrapped to true: " + radioButton.IsWordWrapped);
            
            radioButton.IsWordWrapped = false;
            Console.WriteLine("After setting IsWordWrapped to false: " + radioButton.IsWordWrapped);

            // احفظ المصنف
            workbook.Save("RadioButtonIsWordWrappedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


