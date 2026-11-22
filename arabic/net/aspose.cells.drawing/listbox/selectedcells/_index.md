---
title: "ListBox.SelectedCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBox. تحصل على الخلايا المحددة. تُرجع null إذا لم يتم تعيين نطاق الإدخال أو لم يتم تحديد أي عنصر"
type: docs
url: /ar/net/aspose.cells.drawing/listbox/selectedcells/
---
## ListBox.SelectedCells property

يحصل على الخلايا المحددة. يرجع null إذا لم يتم تعيين نطاق الإدخال أو لم يتم تحديد أي عنصر.

```csharp
public Cell[] SelectedCells { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ListBoxPropertySelectedCellsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات عينة لعناصر ListBox
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // إنشاء ListBox وربطه بنطاق البيانات
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(7, 0, 100, 150, 5, 1);
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            // تحديد عناصر متعددة باستخدام فهارس تبدأ من الصفر
            listBox.SelectedItem(0, true);
            listBox.SelectedItem(2, true);

            // استرجاع وعرض الخلايا المحددة
            Cell[] selectedCells = listBox.SelectedCells;
            Console.WriteLine("Selected Cells Count: " + selectedCells.Length);
            
            // تعديل الخلايا المحددة لإظهار الوصول
            foreach (Cell cell in selectedCells)
            {
                Console.WriteLine("Selected Cell Address: " + cell.Name);
                cell.PutValue("[SELECTED] " + cell.StringValue);
            }

            workbook.Save("ListBoxSelectedCellsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../../aspose.cells/cell/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


