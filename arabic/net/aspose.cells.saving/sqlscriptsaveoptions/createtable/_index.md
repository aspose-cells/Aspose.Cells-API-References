---
title: "SqlScriptSaveOptions.CreateTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SqlScriptSaveOptions. تشير إلى ما إذا كان تصدير SQL لإنشاء الجدول"
type: docs
url: /ar/net/aspose.cells.saving/sqlscriptsaveoptions/createtable/
---
## SqlScriptSaveOptions.CreateTable property

يحدد ما إذا كان تصدير sql لإنشاء جدول.

```csharp
public bool CreateTable { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCreateTableDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // تكوين خيارات تصدير SQL مع تمكين CreateTable
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                CreateTable = true,
                TableName = "Employees",
                HasHeaderRow = true
            };

            // حفظ كسكريبت SQL
            workbook.Save("output.sql", options);
        }
    }
}
```

### انظر أيضًا

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


