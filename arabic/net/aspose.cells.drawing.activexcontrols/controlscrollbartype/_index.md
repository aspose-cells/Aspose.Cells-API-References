---
title: "التعداد ControlScrollBarType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType. يمثل نوع شريط التمرير"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/controlscrollbartype/
---
## ControlScrollBarType enumeration

يمثل نوع شريط التمرير.

```csharp
public enum ControlScrollBarType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | لا يعرض أي أشرطة تمرير. |
| Horizontal | `1` | يعرض شريط تمرير أفقي. |
| BarsVertical | `2` | يعرض شريط تمرير عمودي. |
| BarsBoth | `3` | يعرض كلًا من شريط تمرير أفقي وآخر عمودي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollBarTypeDemo
    {
        public static void ControlScrollBarTypeExample()
        {
            // تهيئة دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم ListBox ActiveX إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            ListBoxActiveXControl listBoxControl = (ListBoxActiveXControl)shape.ActiveXControl;

            // عيّن خاصية ScrollBars لعرض كل من أشرطة التمرير الأفقية والعمودية
            listBoxControl.ScrollBars = ControlScrollBarType.BarsBoth;

            // احفظ المصنف
            workbook.Save("ControlScrollBarTypeExample.xlsx");
            workbook.Save("ControlScrollBarTypeExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


