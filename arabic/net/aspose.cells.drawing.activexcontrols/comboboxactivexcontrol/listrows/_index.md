---
title: "ComboBoxActiveXControl.ListRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ComboBoxActiveXControl. تمثل الحد الأقصى لعدد الصفوف التي تُعرض في القائمة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listrows/
---
## ComboBoxActiveXControl.ListRows property

يمثل الحد الأقصى لعدد الصفوف التي يتم عرضها في القائمة.

```csharp
public int ListRows { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListRowsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ComboBox ActiveX مع معلمات العرض/الارتفاع المناسبة
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 10, 10, 150, 30, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // أضف عناصر نموذجية إلى مربع القائمة باستخدام ListFillRange
            comboBox.ListFillRange = "A1:A7";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");
            worksheet.Cells["A7"].PutValue("Item 7");

            // تعيين خاصية ListRows للتحكم في العناصر المرئية في القائمة المنسدلة
            comboBox.ListRows = 4; // Only show 4 items at a time

            // احفظ المصنف
            workbook.Save("ComboBoxListRowsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


