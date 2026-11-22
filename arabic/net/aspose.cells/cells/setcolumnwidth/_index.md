---
title: "Cells.SetColumnWidth"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُحدد عرض العمود المحدد في العرض العادي"
type: docs
url: /ar/net/aspose.cells/cells/setcolumnwidth/
---
## Cells.SetColumnWidth method

يضبط عرض العمود المحدد في العرض العادي.

```csharp
public void SetColumnWidth(int column, double width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |
| العرض | Double | عرض العمود بوحدة الأحرف. يجب أن يكون عرض العمود بين 0 و 255. |

### ملاحظات

في جداول البيانات، يُقاس عرض العمود بعدد الأحرف لعرض الرقم الأقصى للأرقام 0~9 كما يُظهره خط النمط العادي.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetColumnWidth(0, 25.5);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


