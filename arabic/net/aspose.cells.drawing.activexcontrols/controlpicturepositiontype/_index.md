---
title: "Enum ControlPicturePositionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.ActiveXControls.ControlPicturePositionType. يمثل موقع صورة العنصر بالنسبة للعنوان الخاص به"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/controlpicturepositiontype/
---
## ControlPicturePositionType enumeration

يمثل موقع صورة التحكم بالنسبة إلى تسميته.

```csharp
public enum ControlPicturePositionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| LeftTop | `131072` | الصورة تظهر إلى يسار التسمية. التسمية محاذاة مع أعلى الصورة. |
| LeftCenter | `327683` | الصورة تظهر إلى يسار التسمية. التسمية متمركزة بالنسبة للصورة. |
| LeftBottom | `524294` | الصورة تظهر إلى يسار التسمية. التسمية محاذاة مع أسفل الصورة. |
| RightTop | `2` | الصورة تظهر إلى يمين التسمية. التسمية محاذاة مع أعلى الصورة. |
| RightCenter | `196613` | الصورة تظهر إلى يمين التسمية. التسمية متمركزة بالنسبة للصورة. |
| RightBottom | `393224` | الصورة تظهر إلى يمين التسمية. التسمية محاذاة مع أسفل الصورة. |
| AboveLeft | `393216` | الصورة تظهر فوق التسمية. التسمية محاذاة مع الحافة اليسرى للصورة. |
| AboveCenter | `458753` | الصورة تظهر فوق التسمية. التسمية متمركزة أسفل الصورة. |
| AboveRight | `524290` | الصورة تظهر فوق التسمية. التسمية محاذاة مع الحافة اليمنى للصورة. |
| BelowLeft | `6` | الصورة تظهر أسفل التسمية. التسمية محاذاة مع الحافة اليسرى للصورة. |
| BelowCenter | `65543` | الصورة تظهر أسفل التسمية. التسمية متمركزة فوق الصورة. |
| BelowRight | `131080` | الصورة تظهر أسفل التسمية. التسمية محاذاة مع الحافة اليمنى للصورة. |
| Center | `262148` | الصورة تظهر في وسط التحكم. التسمية متمركزة أفقياً وعمودياً فوق الصورة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassControlPicturePositionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 0, 1, 0, 100, 50);
            ToggleButtonActiveXControl activeXControl = (ToggleButtonActiveXControl)shape.ActiveXControl;

            activeXControl.Caption = "Demo Button";
            activeXControl.PicturePosition = ControlPicturePositionType.AboveLeft;
            activeXControl.IsAutoSize = true;

            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


