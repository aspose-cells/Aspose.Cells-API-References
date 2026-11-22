---
title: "DataSorter.Order1"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorter. تمثل ترتيب الفرز للمفتاح الأول"
type: docs
url: /ar/net/aspose.cells/datasorter/order1/
---
## DataSorter.Order1 property

يمثل ترتيب الفرز للمفتاح الأول.

```csharp
public SortOrder Order1 { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyOrder1Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);

            // حدد خصائص مُرتب البيانات
            DataSorter sorter = workbook.DataSorter;
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // حدد نطاق الفرز
            CellArea area = CellArea.CreateCellArea("A1", "B4");
            
            // تنفيذ الفرز
            sorter.Sort(worksheet.Cells, area);
            
            // احفظ المصنف
            workbook.Save("SortedOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


