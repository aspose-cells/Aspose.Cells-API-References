---
title: "WorksheetCollection.GetNamedRanges"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorksheetCollection. تحصل على جميع النطاقات المسماة المعرفة مسبقًا في جدول البيانات"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/getnamedranges/
---
## WorksheetCollection.GetNamedRanges method

يحصل على جميع النطاقات المسماة المعرفة مسبقًا في جدول البيانات.

```csharp
public Range[] GetNamedRanges()
```

### قيمة الإرجاع

مصفوفة من كائنات Range. إذا كان مرجع الاسم المحدد خارجيًا أو يحتوي على نطاقات متعددة، لن يتم إرجاع كائن Range لهذا الاسم.

يرجع null إذا لم يكن النطاق المسماة موجودًا.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetNamedRangesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بعض النطاقات المسماة للعرض
            worksheet.Cells.CreateRange("A1:B2").Name = "SalesData";
            worksheet.Cells.CreateRange("C3:D4").Name = "Expenses";

            try
            {
                // استدعاء طريقة GetNamedRanges لاسترجاع جميع النطاقات المسماة
                Aspose.Cells.Range[] namedRanges = workbook.Worksheets.GetNamedRanges();

                // عرض المعلومات حول النطاقات المسماة
                Console.WriteLine("Found {0} named ranges:", namedRanges.Length);
                foreach (Aspose.Cells.Range range in namedRanges)
                {
                    Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
                }

                // احفظ المصنف
                workbook.Save("GetNamedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNamedRanges: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


