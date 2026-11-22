---
title: "ComboBoxActiveXControl.ListWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ComboBoxActiveXControl. يحصل على ويضبط العرض بوحدة النقاط"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listwidth/
---
## ComboBoxActiveXControl.ListWidth property

يحصل على العرض بوحدة النقاط ويضبطه.

```csharp
public double ListWidth { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListWidthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لـ ComboBox
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");

            // إضافة عنصر تحكم ComboBox ActiveX مع جميع المعلمات المطلوبة
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                1,  // left
                1,  // top
                100, // width
                30,  // height
                0,   // image width (unused for ComboBox)
                0    // image height (unused for ComboBox)
            );
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // تعيين خاصية ListWidth للتحكم في عرض القائمة المنسدلة
            comboBox.ListWidth = 150;
            comboBox.ListRows = 3;
            comboBox.LinkedCell = "A1:A3";

            // احفظ المصنف
            workbook.Save("ComboBoxListWidthDemo.xlsx");

            Console.WriteLine("ComboBox ListWidth set to: " + comboBox.ListWidth);
        }
    }
}
```

### انظر أيضًا

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


