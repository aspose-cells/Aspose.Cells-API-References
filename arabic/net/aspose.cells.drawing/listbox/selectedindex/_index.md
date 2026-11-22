---
title: "ListBox.SelectedIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBox. تحصل أو تعين رقم الفهرس للعنصر المحدد حاليًا في مربع قائمة أو صندوق اختيار. يبدأ من الصفر"
type: docs
url: /ar/net/aspose.cells.drawing/listbox/selectedindex/
---
## ListBox.SelectedIndex property

يحصل أو يضبط رقم الفهرس للعنصر المحدد حاليًا في مربع قائمة أو مربع اختيار. يبدأ من الصفر.

```csharp
public int SelectedIndex { get; set; }
```

### ملاحظات

-1 presents no item is selected.

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectedIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Item 0");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            
            ListBox listBox = worksheet.Shapes.AddListBox(5, 5, 100, 100, 200, 300);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            listBox.SelectedIndex = 2;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


