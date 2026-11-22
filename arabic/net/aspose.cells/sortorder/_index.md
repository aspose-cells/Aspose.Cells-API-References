---
title: "تعداد SortOrder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.SortOrder. يمثل ترتيب الفرز لنطاق البيانات"
type: docs
url: /ar/net/aspose.cells/sortorder/
---
## SortOrder enumeration

يمثل ترتيب الفرز لنطاق البيانات.

```csharp
public enum SortOrder
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Ascending | `0` | فرز البيانات بترتيب تصاعدي |
| Descending | `1` | فرز البيانات بترتيب تنازلي |
| Natural | `2` | يحافظ على ترتيب البيانات الأصلي دون فرز. ينطبق فقط على بعض السيناريوهات الخاصة مثل PivotTable. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSortOrderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            var workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة للفرز
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(78);
            
            // إنشاء أداة فرز البيانات
            var sorter = workbook.DataSorter;
            
            // تحديد ترتيب الفرز والمفاتيح
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Sort by column B (Score)
            
            // تحديد منطقة الفرز
            var sortArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };
            
            // تنفيذ الفرز
            sorter.Sort(worksheet.Cells, sortArea);
            
            // احفظ المصنف
            workbook.Save("SortedData.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


