---
title: "JsonSaveOptions.ToExcelStruct"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonSaveOptions. تشير إلى ما إذا كان يتم التحويل إلى هيكل JSON لملف Excel"
type: docs
url: /ar/net/aspose.cells/jsonsaveoptions/toexcelstruct/
---
## JsonSaveOptions.ToExcelStruct property

يشير إلى ما إذا كان يتم تحويل ملف Excel إلى بنية JSON.

```csharp
public bool ToExcelStruct { get; set; }
```

### ملاحظات

فقط لتحويل النطاق إلى JSON.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyToExcelStructDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // إنشاء نطاق للتصدير
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

            // تكوين خيارات حفظ JSON باستخدام ToExcelStruct
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ToExcelStruct = true;

            // تصدير النطاق إلى JSON
            string json = range.ToJson(saveOptions);
            Console.WriteLine(json);
        }
    }
}
```

### انظر أيضًا

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


