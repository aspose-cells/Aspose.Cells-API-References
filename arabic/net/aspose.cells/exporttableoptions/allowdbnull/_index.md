---
title: "ExportTableOptions.AllowDBNull"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ExportTableOptions. هذه القيمة تشير إلى ما إذا كان مسموحًا بـ DBNulls في هذا الجدول"
type: docs
url: /ar/net/aspose.cells/exporttableoptions/allowdbnull/
---
## ExportTableOptions.AllowDBNull property

تشير هذه القيمة إلى ما إذا كان مسموحًا بـ DBNulls في هذا الجدول.

```csharp
public bool AllowDBNull { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyAllowDBNullDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي مع بيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة مع بعض الخلايا الفارغة
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue(""); // Empty cell
            worksheet.Cells["B3"].PutValue(25);

            // تصدير مع AllowDBNull = true (الافتراضي)
            ExportTableOptions options1 = new ExportTableOptions
            {
                ExportColumnName = true,
                AllowDBNull = true
            };
            
            DataTable table1 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options1);
            Console.WriteLine("With AllowDBNull=true:");
            Console.WriteLine("Row 2 Name: " + (table1.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table1.Rows[1]["Name"]));

            // تصدير مع AllowDBNull = false
            ExportTableOptions options2 = new ExportTableOptions
            {
                ExportColumnName = true,
                AllowDBNull = false
            };
            
            DataTable table2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, options2);
            Console.WriteLine("\nWith AllowDBNull=false:");
            Console.WriteLine("Row 2 Name: " + (table2.Rows[1]["Name"] == DBNull.Value ? "DBNull" : table2.Rows[1]["Name"]));
        }
    }
}
```

### انظر أيضًا

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


