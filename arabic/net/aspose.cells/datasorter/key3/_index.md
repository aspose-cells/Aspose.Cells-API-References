---
title: "DataSorter.Key3"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorter. تمثل الفهرس الثالث للعمود المرتب الموضع المطلق للعمود A هو 0 B هو 1"
type: docs
url: /ar/net/aspose.cells/datasorter/key3/
---
## DataSorter.Key3 property

يمثل فهرس العمود المرتب الثالث (الموضع المطلق، العمود A هو 0، B هو 1، ...).

```csharp
public int Key3 { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey3Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أضف بيانات تجريبية
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["C1"].PutValue("Grade");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["C2"].PutValue("B");
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["C3"].PutValue("A");
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);
            cells["C4"].PutValue("C");
            cells["A5"].PutValue("Eve");
            cells["B5"].PutValue(92);
            cells["C5"].PutValue("A");

            // إنشاء أداة فرز البيانات
            DataSorter sorter = workbook.DataSorter;
            
            // رتب حسب الدرجة (تنازليًا)، ثم حسب الاسم (تصاعديًا)، ثم حسب التقدير (تنازليًا)
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Column B (Score)
            
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 0; // Column A (Name)
            
            sorter.Order3 = SortOrder.Descending;
            sorter.Key3 = 2; // Column C (Grade)
            
            // فرز نطاق البيانات
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 5, 2));

            // احفظ المصنف
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


