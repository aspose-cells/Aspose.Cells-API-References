---
title: "DataSorter.HasHeaders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorter. تمثل ما إذا كان النطاق يحتوي على رؤوس"
type: docs
url: /ar/net/aspose.cells/datasorter/hasheaders/
---
## DataSorter.HasHeaders property

يمثل ما إذا كان النطاق يحتوي على رؤوس.

```csharp
public bool HasHeaders { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyHasHeadersDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة رؤوس وبيانات عينة
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["B4"].PutValue(12);

            // إنشاء فرّاز بيانات وتعيين HasHeaders إلى true
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true; // This tells the sorter the first row contains headers
            
            // فرز حسب العمود الأول (Fruits) بترتيب تصاعدي
            sorter.AddKey(0, SortOrder.Ascending);
            
            // فرز نطاق البيانات (بما في ذلك الرؤوس)
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "B4"));

            // حفظ دفتر العمل المرتب
            workbook.Save("SortedWithHeaders.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


