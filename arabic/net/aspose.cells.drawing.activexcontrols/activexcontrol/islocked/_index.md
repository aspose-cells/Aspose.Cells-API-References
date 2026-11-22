---
title: "ActiveXControl.IsLocked"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControl. تشير إلى ما إذا كانت البيانات في التحكم مقفلة للتحرير"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrol/islocked/
---
## ActiveXControl.IsLocked property

يشير إلى ما إذا كانت البيانات في العنصر مقفلة للتحرير.

```csharp
public bool IsLocked { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsLockedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // إلغاء قفل جميع الأعمدة باستثناء الأول
            Style style;
            StyleFlag flag;
            for (int i = 0; i <= 255; i++)
            {
                style = sheet.Cells.Columns[(byte)i].GetStyle();
                style.IsLocked = false;
                flag = new StyleFlag();
                flag.Locked = true;
                sheet.Cells.Columns[(byte)i].ApplyStyle(style, flag);
            }

            // قفل العمود الأول
            style = sheet.Cells.Columns[0].GetStyle();
            style.IsLocked = true;
            flag = new StyleFlag();
            flag.Locked = true;
            sheet.Cells.Columns[0].ApplyStyle(style, flag);

            // إضافة عنصر تحكم ActiveX ComboBox
            Shape comboBoxShape = sheet.Shapes.AddActiveXControl(
                ControlType.ComboBox, 
                5, 0, 5, 0, 100, 20);

            // تعيين خصائص عنصر تحكم ActiveX بما في ذلك IsLocked
            ComboBoxActiveXControl comboBox = 
                (ComboBoxActiveXControl)comboBoxShape.ActiveXControl;
            comboBox.IsLocked = false; // Demonstrate IsLocked property
            comboBox.IsVisible = true;
            comboBox.BorderStyle = ControlBorderType.None;

            // حماية ورقة العمل
            sheet.Protect(ProtectionType.All);

            // احفظ المصنف
            wb.Save("ActiveXControlIsLockedDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


