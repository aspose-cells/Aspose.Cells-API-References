---
title: "تعداد ControlSpecialEffectType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.ActiveXControls.ControlSpecialEffectType. يمثل نوع التأثير الخاص"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/controlspecialeffecttype/
---
## ControlSpecialEffectType enumeration

يمثل نوع التأثير الخاص.

```csharp
public enum ControlSpecialEffectType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Flat | `0` | مسطح |
| Raised | `1` | بارز |
| Sunken | `2` | مغروس |
| Etched | `3` | منقوش |
| Bump | `6` | نتوء |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlSpecialEffectTypeDemo
    {
        public static void ControlSpecialEffectTypeExample()
        {
            // تهيئة دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم ActiveX من نوع CheckBox
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
            CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;

            // ضبط خصائص عنصر تحكم ActiveX من نوع CheckBox
            checkBoxControl.Caption = "Example CheckBox";
            checkBoxControl.SpecialEffect = ControlSpecialEffectType.Raised;

            // إضافة عنصر تحكم ActiveX ComboBox
            shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 3, 0, 100, 50);
            ComboBoxActiveXControl comboBoxControl = (ComboBoxActiveXControl)shape.ActiveXControl;

            // تعيين خصائص عنصر تحكم ActiveX ComboBox
            comboBoxControl.SpecialEffect = ControlSpecialEffectType.Sunken;
            comboBoxControl.ListWidth = 100;
            comboBoxControl.ListRows = 5;

            // إضافة عنصر تحكم ActiveX TextBox
            shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 5, 0, 5, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // تعيين خصائص عنصر تحكم ActiveX TextBox
            textBoxControl.Text = "Example TextBox";
            textBoxControl.SpecialEffect = ControlSpecialEffectType.Bump;

            // احفظ المصنف
            workbook.Save("ControlSpecialEffectTypeExample.xlsx");
            workbook.Save("ControlSpecialEffectTypeExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


