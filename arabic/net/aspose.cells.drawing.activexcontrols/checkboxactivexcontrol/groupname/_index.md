---
title: "CheckBoxActiveXControl.GroupName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CheckBoxActiveXControl. تحصل وتضبط اسم المجموعة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/groupname/
---
## CheckBoxActiveXControl.GroupName property

يسترجع ويضبط اسم المجموعة.

```csharp
public string GroupName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم ActiveX من نوع CheckBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // ضبط خاصية GroupName
            checkBox.GroupName = "Sheet1";

            // تحقق وأخرج قيمة GroupName
            Console.WriteLine("CheckBox GroupName: " + checkBox.GroupName);

            // احفظ المصنف
            workbook.Save("CheckBoxActiveXControlGroupNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


