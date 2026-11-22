---
title: "ListBox.SelectionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBox. تحصل أو تعين وضع التحديد للمربع القائمة المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/listbox/selectiontype/
---
## ListBox.SelectionType property

يحصل أو يضبط وضعية التحديد لمربع القائمة المحدد.

```csharp
public SelectionType SelectionType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات نموذجية لمربع القائمة
            sheet.Cells["A1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Finance");
            sheet.Cells["A3"].PutValue("MIS");
            sheet.Cells["A4"].PutValue("R&D");

            // أضف مربع قائمة
            ListBox listBox = sheet.Shapes.AddListBox(1, 0, 2, 0, 100, 80);
            
            // عيّن خصائص مربع القائمة
            listBox.InputRange = "A1:A4";
            listBox.LinkedCell = "B1";
            
            // عرض خاصية SelectionType
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.SelectedIndex = 1; // Select "Finance"

            // احفظ المصنف
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SelectionType](../../selectiontype/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


