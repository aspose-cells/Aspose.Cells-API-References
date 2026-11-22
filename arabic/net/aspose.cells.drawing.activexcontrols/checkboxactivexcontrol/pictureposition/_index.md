---
title: "CheckBoxActiveXControl.PicturePosition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CheckBoxActiveXControl. تحصل وتعيّن موقع صورة التحكم نسبة إلى التسمية التوضيحية"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/pictureposition/
---
## CheckBoxActiveXControl.PicturePosition property

يحصل على موقع صورة التحكم بالنسبة إلى التسمية التوضيحية الخاصة به ويضبطه.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم CheckBox ActiveX مع جميع المعلمات المطلوبة
            var shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CheckBox, 
                10,  // left
                10,  // top
                150, // width
                30,  // height
                0,   // leftOffset
                0    // topOffset
            );
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // قم بتكوين خصائص CheckBox
            checkBox.Caption = "Sample CheckBox";
            checkBox.PicturePosition = ControlPicturePositionType.Center;
            checkBox.IsAutoSize = true;

            // احفظ المصنف
            workbook.Save("CheckBoxPicturePositionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


