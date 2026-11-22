---
title: "ComboBoxActiveXControl.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ComboBoxActiveXControl. تحصل وتعيّن قيمة التحكم"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/value/
---
## ComboBoxActiveXControl.Value property

يحصل على قيمة التحكم ويضبطها.

```csharp
public string Value { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ComboBox ActiveX إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 1, 0, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // حدد الخصائص لـ ComboBox
            comboBox.Value = "Initial Value";
            comboBox.ListFillRange = "A1:A3";
            
            // أضف بعض البيانات النموذجية إلى نطاق القائمة
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // حدّث القيمة المحددة من الخلية المرتبطة
            worksheet.Cells["B1"].PutValue("Option 2");
            worksheet.Shapes.UpdateSelectedValue();

            // عرض الحصول على خاصية Value
            Console.WriteLine("ComboBox Value: " + comboBox.Value);

            // احفظ المصنف
            workbook.Save("ComboBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


