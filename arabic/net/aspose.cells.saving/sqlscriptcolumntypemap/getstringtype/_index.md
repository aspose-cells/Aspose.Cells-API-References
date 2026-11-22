---
title: "SqlScriptColumnTypeMap.GetStringType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SqlScriptColumnTypeMap. يحصل على نوع السلسلة في قاعدة البيانات"
type: docs
url: /ar/net/aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/
---
## SqlScriptColumnTypeMap.GetStringType method

يحصل على النوع النصي في قاعدة البيانات.

```csharp
public virtual string GetStringType()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetStringTypeDemo
    {
        public static void Run()
        {
            // إنشاء مثيل من SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // احصل على وعرض نوع السلسلة الافتراضي
            string stringType = columnTypeMap.GetStringType();
            Console.WriteLine("Default String Type: " + stringType);

            // إنشاء دفتر عمل بسيط يحتوي على بيانات نصية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John Doe");

            // حفظ باستخدام خيارات سكريبت SQL مع استخدام خريطة النوع
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            
            workbook.Save("SqlScriptOutput.sql", saveOptions);
            Console.WriteLine("SQL script saved with string type: " + stringType);
        }
    }
}
```

### انظر أيضًا

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


