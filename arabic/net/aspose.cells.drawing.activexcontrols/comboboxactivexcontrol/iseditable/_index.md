---
title: "ComboBoxActiveXControl.IsEditable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "ComboBoxActiveXControl property. يشير إلى ما إذا كان المستخدم يمكنه الكتابة في العنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/iseditable/
---
## ComboBoxActiveXControl.IsEditable property

يشير إلى ما إذا كان المستخدم يستطيع الكتابة في العنصر.

```csharp
public bool IsEditable { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsEditableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم ComboBox ActiveX باستخدام مجموعة الأشكال
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 5, 0, 100, 30);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // حدد الخصائص لـ ComboBox
            comboBox.IsEditable = true;
            comboBox.Value = "Editable ComboBox";
            comboBox.ColumnCount = 2;
            comboBox.ListRows = 6;
            comboBox.TextColumn = 1;

            // إضافة عناصر إلى ComboBox (باستخدام الخاصية ListFillRange)
            sheet.Cells["A10"].PutValue("Item 1");
            sheet.Cells["B10"].PutValue("Description 1");
            sheet.Cells["A11"].PutValue("Item 2");
            sheet.Cells["B11"].PutValue("Description 2");
            comboBox.ListFillRange = "A10:B11";

            // احفظ المصنف
            workbook.Save("ComboBoxActiveXControl_IsEditableDemo.xlsx");

            // تحقق من الخاصية بعد الحفظ
            Console.WriteLine("IsEditable property value: " + comboBox.IsEditable);
        }
    }
}
```

### انظر أيضًا

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


