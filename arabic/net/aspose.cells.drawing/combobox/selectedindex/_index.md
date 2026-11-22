---
title: "ComboBox.SelectedIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ComboBox. تحصل أو تعين رقم الفهرس للعنصر المحدد حالياً في مربع القائمة أو مربع السرد. يبدأ من الصفر"
type: docs
url: /ar/net/aspose.cells.drawing/combobox/selectedindex/
---
## ComboBox.SelectedIndex property

يحصل أو يضبط رقم الفهرس للعنصر المحدد حاليًا في مربع قائمة أو مربع اختيار. يبدأ من الصفر.

```csharp
public int SelectedIndex { get; set; }
```

### ملاحظات

-1 presents no item is selected.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة لمربع السرد
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // أضف مربع سرد إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 20);
            ComboBox comboBox = (ComboBox)shape;

            // تعيين نطاق الإدخال لمربع القائمة
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // عيّن وعرض الفهرس المحدد
            comboBox.SelectedIndex = 2; // Selects "Item 3" (zero-based index)
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);

            // غيّر الفهرس المحدد وعرضه مرة أخرى
            comboBox.SelectedIndex = 4; // Selects "Item 5"
            Console.WriteLine("\nAfter changing selection:");
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);
        }
    }
}
```

### انظر أيضًا

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


