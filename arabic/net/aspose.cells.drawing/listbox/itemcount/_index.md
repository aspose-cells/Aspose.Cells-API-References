---
title: "ListBox.ItemCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListBox. تحصل على عدد العناصر في مربع القائمة"
type: docs
url: /ar/net/aspose.cells.drawing/listbox/itemcount/
---
## ListBox.ItemCount property

يحصل على عدد العناصر في مربع القائمة.

```csharp
public int ItemCount { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyItemCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("Sheet1");

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Mango");

            // إنشاء مربع قائمة وتعيين الخصائص
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 10, 0, 100, 150);
            listBox.InputRange = "A1:A4";
            
            // إظهار استخدام ItemCount
            int itemCount = listBox.ItemCount;
            Console.WriteLine("ListBox contains {0} items", itemCount);
            
            // ضبط ارتفاع مربع القائمة بناءً على عدد العناصر
            listBox.Height = itemCount * 15;

            workbook.Save("ListBoxItemCountDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


