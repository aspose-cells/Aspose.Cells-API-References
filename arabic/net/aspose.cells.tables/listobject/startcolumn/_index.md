---
title: "ListObject.StartColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. يحصل على العمود الأول للنطاق"
type: docs
url: /ar/net/aspose.cells.tables/listobject/startcolumn/
---
## ListObject.StartColumn property

يحصل على العمود الابتدائي للنطاق.

```csharp
public int StartColumn { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyStartColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء بيانات عينة للجدول
            worksheet.Cells["E5"].PutValue("ID");
            worksheet.Cells["F5"].PutValue("Name");
            worksheet.Cells["G5"].PutValue("Age");
            
            worksheet.Cells["E6"].PutValue(1);
            worksheet.Cells["F6"].PutValue("John");
            worksheet.Cells["G6"].PutValue(30);
            
            worksheet.Cells["E7"].PutValue(2);
            worksheet.Cells["F7"].PutValue("Alice");
            worksheet.Cells["G7"].PutValue(25);

            // إنشاء كائن قائمة (جدول)
            int startRow = 5;
            int startCol = 4; // Column E (0-based index 4)
            int endRow = 7;
            int endCol = 6; // Column G (0-based index 6)
            
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add(startRow, startCol, endRow, endCol, true)];
            
            // عرض خاصية StartColumn
            Console.WriteLine("Table starts at column index: " + table.StartColumn);
            Console.WriteLine("Table starts at column letter: " + CellsHelper.ColumnIndexToName(table.StartColumn));
            
            // احفظ المصنف
            workbook.Save("ListObjectStartColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


