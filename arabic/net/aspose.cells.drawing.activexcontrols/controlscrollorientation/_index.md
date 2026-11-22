---
title: "التعداد ControlScrollOrientation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.ActiveXControls.ControlScrollOrientation. يمثل نوع اتجاه التمرير"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/controlscrollorientation/
---
## ControlScrollOrientation enumeration

يمثل نوع اتجاه التمرير

```csharp
public enum ControlScrollOrientation
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Auto | `3` | يتم عرض التحكم أفقيًا عندما يكون عرض التحكم أكبر من ارتفاعه. يتم عرض التحكم عموديًا في غير ذلك. |
| Vertical | `0` | يتم عرض التحكم عموديًا. |
| Horizontal | `1` | يتم عرض التحكم أفقيًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollOrientationDemo
    {
        public static void ControlScrollOrientationExample()
        {
            // تهيئة دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ScrollBarActiveXControl إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 50);
            ScrollBarActiveXControl activeXControl = (ScrollBarActiveXControl)shape.ActiveXControl;

            // اضبط خصائص ScrollBarActiveXControl
            activeXControl.LargeChange = 5;
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            // عرض ضبط الاتجاه باستخدام تعداد ControlScrollOrientation
            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            // احفظ المصنف
            workbook.Save("ControlScrollOrientationExample.xlsx");
            workbook.Save("ControlScrollOrientationExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


