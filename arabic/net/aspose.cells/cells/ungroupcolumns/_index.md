---
title: "Cells.UngroupColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تفك تجميع الأعمدة"
type: docs
url: /ar/net/aspose.cells/cells/ungroupcolumns/
---
## Cells.UngroupColumns method

يفك تجميع الأعمدة.

```csharp
public void UngroupColumns(int firstIndex, int lastIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | Int32 | فهرس العمود الأول لتفكيك التجميع. |
| lastIndex | Int32 | فهرس العمود الأخير لتفكيك التجميع. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // قم بتجميع الأعمدة أولاً لتوضيح عملية تفكيك التجميع
            worksheet.Cells.GroupColumns(0, 2);

            // تفكيك تجميع الأعمدة (0 إلى 2)
            worksheet.Cells.UngroupColumns(0, 2);

            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


