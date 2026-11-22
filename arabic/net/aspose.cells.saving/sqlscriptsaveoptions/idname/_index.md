---
title: "SqlScriptSaveOptions.IdName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SqlScriptSaveOptions. تحصل وتعيّن اسم عمود المعرف"
type: docs
url: /ar/net/aspose.cells.saving/sqlscriptsaveoptions/idname/
---
## SqlScriptSaveOptions.IdName property

الحصول على وتعيين اسم عمود المعرف.

```csharp
public string IdName { get; set; }
```

### ملاحظات

إذا تم ضبط هذه الخاصية، سيتم إدراج عمود بقيمة عددية صحيحة تتزايد تلقائيًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyIdNameDemo
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

            // تهيئة خيارات تصدير SQL باستخدام IdName
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                CreateTable = true,
                HasHeaderRow = true
            };

            // حفظ كسكريبت SQL
            workbook.Save("Employees.sql", saveOptions);

            Console.WriteLine("SQL script exported with IdName property");
        }
    }
}
```

### انظر أيضًا

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


