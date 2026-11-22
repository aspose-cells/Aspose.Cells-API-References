---
title: "WorksheetCollection.SortNames"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorksheetCollection. يقوم بترتيب الأسماء المعرفة"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/sortnames/
---
## WorksheetCollection.SortNames method

يبدل الورقتين.

```csharp
public void SortNames()
```

### ملاحظات

إذا قمت بإنشاء عدد كبير من النطاقات المسماة في ملف Excel، يرجى استدعاء هذه الطريقة بعد إنشاء جميع النطاقات المسماة وقبل الحفظ

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSortNamesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة بعض النطاقات المسماة
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test1");
            worksheet.Cells.CreateRange("A1").Name = "Range2";
            worksheet.Cells["B1"].PutValue("Test2");
            worksheet.Cells.CreateRange("B1").Name = "Range1";
            
            // عرض الأسماء قبل الفرز
            Console.WriteLine("Before sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // فرز الأسماء
            workbook.Worksheets.SortNames();
            
            // عرض الأسماء بعد الفرز
            Console.WriteLine("\nAfter sorting:");
            foreach (Name name in workbook.Worksheets.Names)
            {
                Console.WriteLine(name.RefersTo);
            }
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


