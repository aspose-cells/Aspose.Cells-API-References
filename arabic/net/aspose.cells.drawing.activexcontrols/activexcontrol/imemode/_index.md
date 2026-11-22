---
title: "ActiveXControl.IMEMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControl. تحصل وتضبط وضع التشغيل الافتراضي لمحرر طريقة الإدخال للعنصر عند استلامه للتركيز"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrol/imemode/
---
## ActiveXControl.IMEMode property

يحصل على وضع وقت التشغيل الافتراضي لمحرر طريقة الإدخال للعنصر عند استلامه للتركيز ويضبطه.

```csharp
public InputMethodEditorMode IMEMode { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIMEModeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم ActiveX ToggleButton مع إحداثيات صحيحة
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ToggleButton, 
                1, 1,  // Upper-left row/column
                1, 1,  // Upper-left row/column offsets
                100, 50);  // Width and height
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // تعيين الخصائص بما في ذلك IMEMode
            toggleButton.Caption = "ToggleButton1";
            toggleButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            toggleButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            toggleButton.IMEMode = InputMethodEditorMode.NoControl;

            // التحقق وإخراج خاصية IMEMode
            Console.WriteLine("ToggleButton IMEMode: " + toggleButton.IMEMode);

            // احفظ المصنف
            workbook.Save("ActiveXControlIMEModeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [InputMethodEditorMode](../../inputmethodeditormode/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


