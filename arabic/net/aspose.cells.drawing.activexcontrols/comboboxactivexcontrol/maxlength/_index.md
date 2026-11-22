---
title: "ComboBoxActiveXControl.MaxLength"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "ComboBoxActiveXControl property. يحصل على الحد الأقصى لعدد الأحرف ويضبطه"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/maxlength/
---
## ComboBoxActiveXControl.MaxLength property

يحصل على الحد الأقصى لعدد الأحرف ويضبطه

```csharp
public int MaxLength { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyMaxLengthDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ComboBox ActiveX إلى ورقة العمل
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                5, 0, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // تعيين خاصية MaxLength وغيرها من الخصائص الأساسية
            comboBox.MaxLength = 10; // Restrict input to 10 characters
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;
            comboBox.Value = "Test";

            // احفظ المصنف
            workbook.Save("ComboBoxMaxLengthDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


