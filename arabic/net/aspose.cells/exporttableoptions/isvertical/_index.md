---
title: "ExportTableOptions.IsVertical"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportTableOptions. True إذا كان الصف في ملف Workbook يمثل صفًا في DataTable. False إذا كان العمود في ملف Workbook يمثل صفًا في DataTable"
type: docs
url: /ar/net/aspose.cells/exporttableoptions/isvertical/
---
## ExportTableOptions.IsVertical property

True إذا كان الصف في ملف Workbook يمثل صفًا في DataTable. False إذا كان العمود في ملف Workbook يمثل صفًا في DataTable.

```csharp
public bool IsVertical { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyIsVerticalDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء بيانات عينة في ورقة العمل
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(25);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(30);

            // إنشاء DataTable
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));

            // تعيين ExportTableOptions مع IsVertical = true
            ExportTableOptions options = new ExportTableOptions();
            options.IsVertical = true;
            options.ExportColumnName = true;
            options.DataTable = dt;

            // تصدير البيانات عموديًا
            cells.ExportDataTable(0, 0, 2, 2, options);

            // عرض DataTable المُصدَّر
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


