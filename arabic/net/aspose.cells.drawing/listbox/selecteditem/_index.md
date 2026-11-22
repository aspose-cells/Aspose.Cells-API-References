---
title: "ListBox.SelectedItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListBox. تحدد ما إذا كان العنصر محددًا"
type: docs
url: /ar/net/aspose.cells.drawing/listbox/selecteditem/
---
## ListBox.SelectedItem method

يضبط ما إذا كان العنصر محددًا

```csharp
public void SelectedItem(int itemIndex, bool isSelected)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| itemIndex | Int32 | فهرس العنصر |
| isSelected | منطقي | ما إذا كان العنصر محددًا. يعني True أن هذا العنصر يجب أن يكون محددًا. يعني False أن هذا العنصر يجب أن يكون غير محدد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ListBoxMethodSelectedItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ عناصر القائمة
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i, 0].Value = $"Item {i + 1}";
            }

            // إنشاء مربع قائمة
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 150, 100) as ListBox;
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            try
            {
                // تحديد وإلغاء تحديد العناصر
                listBox.SelectedItem(2, true);  // Select third item (index 2)
                listBox.SelectedItem(0, true);   // Select first item (index 0)
                listBox.SelectedItem(2, false); // Deselect third item

                // تحقق من الاختيارات
                Console.WriteLine($"Item 0 selected: {listBox.IsSelected(0)}");
                Console.WriteLine($"Item 2 selected: {listBox.IsSelected(2)}");

                // عرض الخلايا المحددة
                Console.WriteLine("\nSelected Items:");
                foreach (Cell cell in listBox.SelectedCells)
                {
                    Console.WriteLine(cell.Value);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ListBoxMethodSelectedItemWithInt32BooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


