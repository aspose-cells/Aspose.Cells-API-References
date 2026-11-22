---
title: "DataSorter.Key1"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorter. تمثل فهرس العمود الأول المرتب (الموضع المطلق، العمود A هو 0 والعمود B هو 1)"
type: docs
url: /ar/net/aspose.cells/datasorter/key1/
---
## DataSorter.Key1 property

يمثل فهرس العمود المرتب الأول (الموضع المطلق، العمود A هو 0، B هو 1، ...).

```csharp
public int Key1 { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKey1Demo
    {
        public static void Run()
        {
            // إنشاء مصنف وإضافة بيانات نموذجية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أضف بيانات تجريبية
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Score");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(85);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(92);
            cells["A4"].PutValue("Bob");
            cells["B4"].PutValue(78);

            // إنشاء مُرتّب بيانات وتعيين Key1 للفرز حسب عمود Score (العمود B)
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 1; // Column index 1 (B)
            sorter.Order1 = SortOrder.Descending;

            // تحديد منطقة الفرز (الصفوف 1-4، جميع أعمدة البيانات)
            CellArea sortArea = new CellArea();
            sortArea.StartRow = 1;
            sortArea.EndRow = 4;
            sortArea.StartColumn = 0;
            sortArea.EndColumn = cells.MaxDataColumn;

            // تنفيذ الفرز
            sorter.Sort(cells, sortArea);

            // حفظ النتيجة
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


