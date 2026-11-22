---
title: "RowCollection.GetRowByIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة RowCollection. تحصل على كائن الصف وفقًا للموقع في القائمة"
type: docs
url: /ar/net/aspose.cells/rowcollection/getrowbyindex/
---
## RowCollection.GetRowByIndex method

يحصل على كائن الصف وفقًا للموقع في القائمة.

```csharp
public Row GetRowByIndex(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | الموقع. |

### قيمة الإرجاع

كائن Row في الموقع المعطى.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetRowByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // الحصول على الصف حسب الفهرس (بدءًا من الصفر)
            Row row = sheet.Cells.Rows.GetRowByIndex(0);
            
            if (row == null)
            {
                Console.WriteLine("Row at index 0 is null (not created yet)");
            }
            else
            {
                Console.WriteLine("Row at index 0 exists");
            }
        }
    }
}
```

### انظر أيضًا

* class [Row](../../row/)
* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


