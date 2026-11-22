---
title: "ColumnCollection.GetByIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ColumnCollection. يحصل على كائن العمود حسب الفهرس"
type: docs
url: /ar/net/aspose.cells/columncollection/getbyindex/
---
## ColumnCollection.GetByIndex method

يحصل على كائن العمود حسب الفهرس.

```csharp
[Obsolete("Use Columns.GetColumnByIndex() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Column GetByIndex(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 |  |

### قيمة الإرجاع

يرجع كائن العمود.

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهملًا. بدلاً من ذلك، يرجى استخدام طريقة Columns.GetColumnByIndex(). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2010. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء أعمدة في المجموعة عن طريق ضبط العرض
            worksheet.Cells.Columns[0].Width = 15;  // Column 0
            worksheet.Cells.Columns[2].Width = 20;  // Column 2
            worksheet.Cells.Columns[4].Width = 25;  // Column 4

            try
            {
                // احصل على العمود الثاني من ColumnCollection (الفهرس 1)
                Column column = worksheet.Cells.Columns.GetByIndex(1);

                Console.WriteLine($"Retrieved column at collection index 1");
                Console.WriteLine($"Worksheet column index: {column.Index}");
                Console.WriteLine($"Original width: {column.Width}");

                // تعديل العمود المسترجع
                column.Width = 35;
                Console.WriteLine($"Updated width: {column.Width}");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ColumnCollectionGetByIndexDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


