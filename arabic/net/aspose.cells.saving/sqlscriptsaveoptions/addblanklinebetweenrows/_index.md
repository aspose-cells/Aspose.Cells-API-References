---
title: "SqlScriptSaveOptions.AddBlankLineBetweenRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SqlScriptSaveOptions. إدراج سطر فارغ بين كل بيانات"
type: docs
url: /ar/net/aspose.cells.saving/sqlscriptsaveoptions/addblanklinebetweenrows/
---
## SqlScriptSaveOptions.AddBlankLineBetweenRows property

إدراج سطر فارغ بين كل بيانات.

```csharp
public bool AddBlankLineBetweenRows { get; set; }
```

### ملاحظات

إذا كان [`Separator`](../separator/) هو '\n' ، فمن الأفضل ضبط هذه الخاصية كصحيح لزيادة قابلية القراءة.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyAddBlankLineBetweenRowsDemo
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
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                OperatorType = SqlScriptOperatorType.Insert,
                TableName = "Employees",
                IdName = "ID",
                AddBlankLineBetweenRows = true,
                CreateTable = true
            };

            // حفظ إلى تدفق الذاكرة والحصول على سكريبت SQL كسلسلة
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string sqlScript = reader.ReadToEnd();
                    Console.WriteLine("SQL script generated with blank lines between rows:");
                    Console.WriteLine(sqlScript);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


