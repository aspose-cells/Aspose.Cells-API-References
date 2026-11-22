---
title: "ComboBox.SelectedValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ComboBox. تحصل على القيمة المحددة لمربع السرد"
type: docs
url: /ar/net/aspose.cells.drawing/combobox/selectedvalue/
---
## ComboBox.SelectedValue property

يحصل على القيمة المحددة لمربع combox.

```csharp
public string SelectedValue { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء ComboBox وإضافة العناصر
            Aspose.Cells.Drawing.ComboBox comboBox = (Aspose.Cells.Drawing.ComboBox)worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 50);
            comboBox.LinkedCell = "A1";
            comboBox.SetInputRange("B1:B4", false, false);
            
            // تعيين القيم في نطاق الإدخال
            worksheet.Cells["B1"].PutValue("a");
            worksheet.Cells["B2"].PutValue("b");
            worksheet.Cells["B3"].PutValue("c");
            worksheet.Cells["B4"].PutValue("d");

            // عرض SelectedValue (خاصية للقراءة فقط)
            Console.WriteLine("SelectedValue: " + comboBox.SelectedValue);

            // احفظ المصنف
            workbook.Save("ComboBoxDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


