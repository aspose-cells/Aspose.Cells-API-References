---
title: "CellsHelper.RowNameToIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. تحصل على فهرس الصف وفقًا لاسم الصف"
type: docs
url: /ar/net/aspose.cells/cellshelper/rownametoindex/
---
## CellsHelper.RowNameToIndex method

يحصل على مؤشر الصف وفقًا لاسم الصف.

```csharp
public static int RowNameToIndex(string rowName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اسم الصف | String | اسم الصف. |

### قيمة الإرجاع

فهرس الصف.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodRowNameToIndexWithStringDemo
    {
        public static void Run()
        {
            string rowName = "11";
            int rowIndex = CellsHelper.RowNameToIndex(rowName);
            Console.WriteLine("Row name '{0}' converted to index: {1}", rowName, rowIndex);
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


