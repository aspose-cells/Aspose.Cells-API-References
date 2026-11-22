---
title: "JsonSaveOptions.Indent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonSaveOptions. تشير إلى المسافة البادئة"
type: docs
url: /ar/net/aspose.cells/jsonsaveoptions/indent/
---
## JsonSaveOptions.Indent property

يشير إلى المسافة البادئة.

```csharp
public string Indent { get; set; }
```

### ملاحظات

إذا كانت المسافة البادئة فارغة أو null، فإن JSON المُصدَّر غير مُنسق.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // تكوين خيارات حفظ JSON مع المسافة البادئة
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                Indent = "    ", // 4 spaces for indentation
                ExportArea = new CellArea { StartRow = 0, EndRow = 3, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true
            };

            // احفظ بمخرجات JSON ذات مسافة بادئة
            workbook.Save("IndentedJsonOutput.json", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


