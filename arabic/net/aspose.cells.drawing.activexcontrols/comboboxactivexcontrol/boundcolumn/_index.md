---
title: "ComboBoxActiveXControl.BoundColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "ComboBoxActiveXControl property. يمثل الطريقة التي يتم بها تحديد خاصية Value لعنصر ComboBox أو ListBox عندما تكون قيمة خاصية MultiSelect هي fmMultiSelectSingle"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/boundcolumn/
---
## ComboBoxActiveXControl.BoundColumn property

يمثّل كيفية تحديد خاصية Value لعنصر ComboBox أو ListBox عندما تكون قيمة خاصية MultiSelect هي (fmMultiSelectSingle).

```csharp
public int BoundColumn { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBoundColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // إضافة عنصر تحكم ActiveX ComboBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 5, 0, 1, 0, 150, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // تكوين ComboBox
            comboBox.ListFillRange = "A1:B4";
            comboBox.ColumnCount = 2;
            comboBox.BoundColumn = 0; // Bind to the ID column (column index 0)
            comboBox.TextColumn = 1; // Display the Name column (column index 1)

            // احفظ المصنف
            workbook.Save("ComboBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ComboBox BoundColumn set to: " + comboBox.BoundColumn);
        }
    }
}
```

### انظر أيضًا

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


