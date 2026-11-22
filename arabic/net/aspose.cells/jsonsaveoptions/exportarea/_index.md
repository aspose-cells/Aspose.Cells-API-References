---
title: "JsonSaveOptions.ExportArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonSaveOptions. تحصل أو تعيّن نطاق التصدير"
type: docs
url: /ar/net/aspose.cells/jsonsaveoptions/exportarea/
---
## JsonSaveOptions.ExportArea property

يحصل أو يعيّن نطاق التصدير.

```csharp
public CellArea ExportArea { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات العينة
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // تكوين خيارات حفظ JSON باستخدام ExportArea
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 }
            };

            // حفظ باستخدام نطاق التصدير المحدد (A1:B3)
            workbook.Save("JsonExportAreaDemo.json", saveOptions);
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


