---
title: "ListBoxActiveXControl.BoundColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBoxActiveXControl. تمثل كيفية تحديد خاصية Value لـ ComboBox أو ListBox عندما تكون قيمة خاصية MultiSelect هي fmMultiSelectSingle"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/boundcolumn/
---
## ListBoxActiveXControl.BoundColumn property

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
    public class ListBoxActiveXControlPropertyBoundColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // أضف عنصر تحكم ListBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 150, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // تكوين خصائص ListBox
            listBox.ColumnCount = 2;
            listBox.ListFillRange = "A1:B4";
            
            // عيّن BoundColumn إلى 0 (عمود المعرف) - سيكون هذا هو القيمة التي تُرجع عند اختيار عنصر
            listBox.BoundColumn = 0;
            
            // عيّن TextColumn إلى 1 (عمود الاسم) - سيتم عرض ذلك في القائمة
            listBox.TextColumn = 1;

            // احفظ المصنف
            workbook.Save("ListBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ListBox BoundColumn set to: " + listBox.BoundColumn);
        }
    }
}
```

### انظر أيضًا

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


