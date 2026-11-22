---
title: "Cell.GetTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحصل على الجدول الذي يحتوي على هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/gettable/
---
## Cell.GetTable method

يحصل على الجدول الذي يحتوي على هذه الخلية.

```csharp
public ListObject GetTable()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellMethodGetTableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أنشئ جدولًا يحتوي على رؤوس وبيانات
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);

            // أنشئ ListObject (جدول) من نطاق البيانات
            int tableIndex = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // أظهر طريقة GetTable
            Cell cellInTable = cells["B2"];
            ListObject resultTable = cellInTable.GetTable();
            
            Console.WriteLine("Table found: " + (resultTable != null));
            Console.WriteLine("Table range: " + resultTable.StartRow + "," + resultTable.StartColumn + 
                            " to " + resultTable.EndRow + "," + resultTable.EndColumn);
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../../../aspose.cells.tables/listobject/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


