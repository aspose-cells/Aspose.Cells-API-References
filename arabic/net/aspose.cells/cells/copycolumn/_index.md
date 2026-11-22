---
title: "Cells.CopyColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تنسخ البيانات والتنسيقات لعمود كامل"
type: docs
url: /ar/net/aspose.cells/cells/copycolumn/
---
## Cells.CopyColumn method

ينسخ البيانات والتنسيقات لعمود كامل.

```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceCells | الخلايا | كائن Source Cells يحتوي على البيانات والتنسيقات للنسخ. |
| sourceColumnIndex | Int32 | مؤشر العمود المصدر. |
| destinationColumnIndex | Int32 | مؤشر العمود الوجهة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل المصدر وتعبئة البيانات
            Workbook wbSrc = new Workbook();
            Cells cellsSrc = wbSrc.Worksheets[0].Cells;
            cellsSrc[0, 255].PutValue(1);
            cellsSrc[1, 255].PutValue(true);
            cellsSrc[2, 255].PutValue("abc");
            cellsSrc[3, 255].PutValue(false);
            cellsSrc[65535, 255].PutValue(2.56);

            // إنشاء دفتر عمل هدف
            Workbook wbDest = new Workbook();
            Cells cellsDest = wbDest.Worksheets[0].Cells;

            // نسخ العمود من المصدر إلى الوجهة
            cellsDest.CopyColumn(cellsSrc, 255, 0);

            // حفظ النتيجة
            wbDest.Save("outputCopyColumn.xlsx");
            
            Console.WriteLine("Column copied successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


