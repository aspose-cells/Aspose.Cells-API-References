---
title: "CellsHelper.ColumnNameToIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. تحصل على فهرس العمود وفقًا لاسم العمود"
type: docs
url: /ar/net/aspose.cells/cellshelper/columnnametoindex/
---
## CellsHelper.ColumnNameToIndex method

يحصل على مؤشر العمود وفقًا لاسم العمود.

```csharp
public static int ColumnNameToIndex(string columnName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnName | String | اسم العمود. |

### قيمة الإرجاع

فهرس العمود.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnNameToIndexWithStringDemo
    {
        public static void Run()
        {
            int columnIndex = CellsHelper.ColumnNameToIndex("BAA");
            string columnName = CellsHelper.ColumnIndexToName(columnIndex);
            
            Console.WriteLine("Column Name: " + columnName);
            Console.WriteLine("Column Index: " + columnIndex);
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


