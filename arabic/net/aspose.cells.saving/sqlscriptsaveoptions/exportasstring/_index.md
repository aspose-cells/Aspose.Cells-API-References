---
title: "SqlScriptSaveOptions.ExportAsString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SqlScriptSaveOptions. تشير إلى ما إذا كان تصدير جميع البيانات كقيمة نصية"
type: docs
url: /ar/net/aspose.cells.saving/sqlscriptsaveoptions/exportasstring/
---
## SqlScriptSaveOptions.ExportAsString property

يحدد ما إذا كان تصدير جميع البيانات كقيمة نصية.

```csharp
public bool ExportAsString { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // تكوين خيارات تصدير SQL
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                ExportAsString = true, // Demonstrating ExportAsString property
                HasHeaderRow = true
            };

            // حفظ مع تمكين تصدير النص
            workbook.Save("ExportAsString_True.sql", saveOptions);

            // تغيير إلى false وحفظ مرة أخرى
            saveOptions.ExportAsString = false;
            workbook.Save("ExportAsString_False.sql", saveOptions);

            Console.WriteLine("SQL scripts saved with different ExportAsString settings.");
        }
    }
}
```

### انظر أيضًا

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


