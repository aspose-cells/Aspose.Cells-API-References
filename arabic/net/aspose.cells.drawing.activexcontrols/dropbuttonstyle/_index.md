---
title: "Enum DropButtonStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.ActiveXControls.DropButtonStyle. يمثل الرمز المعروض على زر السقوط"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/dropbuttonstyle/
---
## DropButtonStyle enumeration

يمثل الرمز المعروض على زر السقوط.

```csharp
public enum DropButtonStyle
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Plain | `0` | يعرض زرًا بدون رمز. |
| Arrow | `1` | يعرض زرًا بسهم أسفل. |
| Ellipsis | `2` | يعرض زرًا بثلاث نقاط (...). |
| Reduce | `3` | يعرض زرًا بخط أفقي يشبه حرف الشرطة السفلية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class DropButtonStyleDemo
    {
        public static void DropButtonStyleExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ComboBox ActiveX إلى ورقة العمل
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // حدد الخصائص لـ ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow; // Set the drop button style to Arrow

            // إضافة بعض العناصر إلى ComboBox
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            comboBox.ListFillRange = "A1:A4";

            // احفظ المصنف
            workbook.Save("DropButtonStyleExample.xlsx");
            workbook.Save("DropButtonStyleExample.pdf");

            // إخراج DropButtonStyle المستخدم
            Console.WriteLine("DropButtonStyle set to: " + comboBox.DropButtonStyle);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


