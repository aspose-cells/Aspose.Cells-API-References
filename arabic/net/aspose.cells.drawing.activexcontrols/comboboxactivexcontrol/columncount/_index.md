---
title: "ComboBoxActiveXControl.ColumnCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ComboBoxActiveXControl. تمثل عدد الأعمدة التي سيتم عرضها في ComboBox أو ListBox"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/columncount/
---
## ComboBoxActiveXControl.ColumnCount property

يمثّل عدد الأعمدة التي تُعرض في عنصر ComboBox أو ListBox.

```csharp
public int ColumnCount { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyColumnCountDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // إضافة عنصر تحكم ComboBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // تعيين خاصية ColumnCount وغيرها من الخصائص
            comboBox.ColumnCount = 1;
            comboBox.ListWidth = 100;
            comboBox.Value = "Apple;Banana;Cherry";

            // احفظ المصنف
            workbook.Save("ComboBoxColumnCountDemo.xlsx");

            Console.WriteLine("ComboBox with ColumnCount=1 has been created and saved.");
        }
    }
}
```

### انظر أيضًا

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


