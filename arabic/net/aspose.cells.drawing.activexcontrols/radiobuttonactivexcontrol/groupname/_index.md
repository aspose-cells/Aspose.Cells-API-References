---
title: "RadioButtonActiveXControl.GroupName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RadioButtonActiveXControl. يسترجع ويضبط اسم المجموعة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/groupname/
---
## RadioButtonActiveXControl.GroupName property

يسترجع ويضبط اسم المجموعة.

```csharp
public string GroupName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصرين RadioButton ActiveX
            var shape1 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 30);
            var radio1 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape1.ActiveXControl;
            
            var shape2 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 50, 100, 30);
            var radio2 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape2.ActiveXControl;

            // تعيين نفس اسم المجموعة لجعلها متعارضة
            radio1.GroupName = "RadioGroup1";
            radio2.GroupName = "RadioGroup1";

            // تعيين التسميات
            radio1.Caption = "Option 1";
            radio2.Caption = "Option 2";

            // احفظ المصنف
            workbook.Save("RadioButtonGroupDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


