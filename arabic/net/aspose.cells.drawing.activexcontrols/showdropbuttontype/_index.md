---
title: "تعداد ShowDropButtonType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ShowDropButtonType enum. يحدد متى يتم إظهار زر السقوط"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/showdropbuttontype/
---
## ShowDropButtonType enumeration

يحدد متى يتم إظهار زر السقوط

```csharp
public enum ShowDropButtonType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Never | `0` | لا تُظهر زر السقوط أبداً. |
| Focus | `1` | أظهر زر السقوط عندما يكون العنصر في حالة التركيز. |
| Always | `2` | اعرض زر السقوط دائماً. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ShowDropButtonTypeDemo
    {
        public static void ShowDropButtonTypeExample()
        {
            // تهيئة دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ComboBox ActiveX إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // ضبط الخصائص لعنصر تحكم ActiveX من نوع ComboBox
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus; // Show drop button when the control has focus
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;

            // إضافة بعض العناصر إلى ComboBox
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // احفظ المصنف
            workbook.Save("ShowDropButtonTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


