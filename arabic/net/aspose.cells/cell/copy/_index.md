---
title: "Cell.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تنسخ البيانات من خلية مصدر"
type: docs
url: /ar/net/aspose.cells/cell/copy/
---
## Cell.Copy method

ينسخ البيانات من خلية المصدر.

```csharp
public void Copy(Cell cell)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cell | Cell | كائن [`Cell`](../) المصدر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCopyWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين القيم والأنماط في الخلية المصدر
            Cell sourceCell = cells["A1"];
            sourceCell.PutValue("Source Value");
            sourceCell.GetStyle().Font.IsBold = true;

            // إنشاء خلية وجهة
            Cell destCell = cells["B1"];

            // نسخ من المصدر إلى الوجهة
            destCell.Copy(sourceCell);

            // تحقق من النسخة
            Console.WriteLine("Destination cell value: " + destCell.StringValue);
            Console.WriteLine("Destination cell bold status: " + destCell.GetStyle().Font.IsBold);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


