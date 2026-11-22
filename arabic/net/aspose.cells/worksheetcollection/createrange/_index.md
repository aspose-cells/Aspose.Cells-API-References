---
title: "WorksheetCollection.CreateRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorksheetCollection. تنشئ كائن Range من عنوان النطاق"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/createrange/
---
## WorksheetCollection.CreateRange method

ينشئ كائن [`Range`](../../range/) من عنوان النطاق.

```csharp
public Range CreateRange(string address, int sheetIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| address | String | عنوان النطاق. |
| sheetIndex | Int32 | فهرس الورقة. |

### قيمة الإرجاع

كائن [`Range`](../../range/)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ بعض بيانات العينة
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 6; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // إنشاء نطاق باستخدام عنوان نصي وفهرس الورقة
            Aspose.Cells.Range range = workbook.Worksheets.CreateRange("A1:F10", 0);

            // عرض استخدام النطاق
            Console.WriteLine($"Range has {range.RowCount} rows and {range.ColumnCount} columns");
            Console.WriteLine($"First cell value: {range[0, 0].StringValue}");
            Console.WriteLine($"Last cell value: {range[9, 5].StringValue}");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


