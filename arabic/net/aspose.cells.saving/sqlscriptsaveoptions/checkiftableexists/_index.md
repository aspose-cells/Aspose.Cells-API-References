---
title: "SqlScriptSaveOptions.CheckIfTableExists"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SqlScriptSaveOptions. تحقق مما إذا كان اسم الجدول موجودًا قبل الإنشاء"
type: docs
url: /ar/net/aspose.cells.saving/sqlscriptsaveoptions/checkiftableexists/
---
## SqlScriptSaveOptions.CheckIfTableExists property

تحقق مما إذا كان اسم الجدول موجودًا قبل الإنشاء

```csharp
public bool CheckIfTableExists { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCheckIfTableExistsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي مع بيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // تكوين خيارات حفظ SQL
            SqlScriptSaveOptions sqlOptions = new SqlScriptSaveOptions();
            sqlOptions.CreateTable = true;
            sqlOptions.CheckIfTableExists = true;
            sqlOptions.OperatorType = SqlScriptOperatorType.Insert;

            // حفظ إلى ملف سكريبت SQL
            workbook.Save("output.sql", sqlOptions);

            // قراءة وإخراج SQL المُنشأ
            string sqlScript = System.IO.File.ReadAllText("output.sql");
            Console.WriteLine("Generated SQL Script:");
            Console.WriteLine(sqlScript);
        }
    }
}
```

### انظر أيضًا

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


