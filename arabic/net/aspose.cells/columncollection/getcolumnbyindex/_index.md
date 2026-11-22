---
title: "ColumnCollection.GetColumnByIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ColumnCollection. يحصل على كائن Column حسب الموضع في القائمة"
type: docs
url: /ar/net/aspose.cells/columncollection/getcolumnbyindex/
---
## ColumnCollection.GetColumnByIndex method

يحصل على كائن [`Column`](../../column/) حسب الموضع في القائمة.

```csharp
public Column GetColumnByIndex(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | الموضع في القائمة. |

### قيمة الإرجاع

يرجع كائن العمود.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetColumnByIndexWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة إلى العمود A
            worksheet.Cells["A1"].Value = "Aspose.Cells Column Demo";

            try
            {
                // احصل على مرجع مجموعة الأعمدة
                ColumnCollection columns = worksheet.Cells.Columns;

                // الوصول إلى العمود عند الفهرس 0 (العمود A) باستخدام GetColumnByIndex
                Column column = columns.GetColumnByIndex(0);

                // عدّل عرض العمود لتوضيح الوصول إلى العمود
                column.Width = 25;

                Console.WriteLine("Modified width of column at index 0 (Column A) to 25 characters.");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid column index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("ColumnCollectionMethodGetColumnByIndexWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


