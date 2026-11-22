---
title: "RowCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة RowCollection. احذف عنصر الصف في الموضع الفهرسي المحدد في هذه المجموعة"
type: docs
url: /ar/net/aspose.cells/rowcollection/removeat/
---
## RowCollection.RemoveAt method

أزل عنصر الصف في الفهرس (الموقع) المحدد في هذه المجموعة.

```csharp
public void RemoveAt(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| index | Int32 | فهرس (مبني على الصفر) (الموضع، ليس [`Index`](../../row/index/)) لعنصر الصف الموجود في هذه المجموعة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات إلى الخلايا في الصفوف القليلة الأولى
            worksheet.Cells["A1"].PutValue("Row 1");
            worksheet.Cells["A2"].PutValue("Row 2");
            worksheet.Cells["A3"].PutValue("Row 3");
            worksheet.Cells["A4"].PutValue("Row 4");

            // اعرض عدد الصفوف الأولي
            Console.WriteLine($"Initial row count: {worksheet.Cells.Rows.Count}");

            try
            {
                // استدعِ طريقة RemoveAt لإزالة الصف عند الفهرس 1 (الصف الثاني)
                worksheet.Cells.Rows.RemoveAt(1);

                Console.WriteLine("Method executed successfully. Row at index 1 removed.");

                // اعرض عدد الصفوف المحدث
                Console.WriteLine($"Updated row count: {worksheet.Cells.Rows.Count}");

                // أظهر التأثير - يجب إزالة الصف 2، يصبح الصف 3 هو الصف 2
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("RowCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


