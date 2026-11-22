---
title: "ComboBoxActiveXControl.TextColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ComboBoxActiveXControl. تمثل العمود في ComboBox أو ListBox الذي يُعرض للمستخدم"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/textcolumn/
---
## ComboBoxActiveXControl.TextColumn property

يمثل العمود في ComboBox أو ListBox الذي يُعرض للمستخدم.

```csharp
public int TextColumn { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyTextColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم ComboBox ActiveX مع جميع المعلمات المطلوبة
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                10, 10, 150, 30, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // إعداد خصائص صندوق القائمة
            comboBox.ColumnCount = 2;
            comboBox.ListRows = 5;
            
            // إضافة عناصر باستخدام ListFillRange (بديل لـ AddItem)
            worksheet.Cells["A1"].PutValue("Item1");
            worksheet.Cells["B1"].PutValue("Description1");
            worksheet.Cells["A2"].PutValue("Item2");
            worksheet.Cells["B2"].PutValue("Description2");
            worksheet.Cells["A3"].PutValue("Item3");
            worksheet.Cells["B3"].PutValue("Description3");
            comboBox.ListFillRange = "A1:B3";

            // عرض خاصية TextColumn
            comboBox.TextColumn = 2; // Display second column (descriptions) as text
            comboBox.BoundColumn = 1; // But bind to first column (items)

            // احفظ المصنف
            workbook.Save("ComboBoxTextColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


