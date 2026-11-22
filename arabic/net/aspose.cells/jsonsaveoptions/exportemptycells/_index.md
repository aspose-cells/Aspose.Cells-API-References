---
title: "JsonSaveOptions.ExportEmptyCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية JsonSaveOptions. تشير إلى ما إذا كان سيتم تصدير الخلايا الفارغة كقيمة null"
type: docs
url: /ar/net/aspose.cells/jsonsaveoptions/exportemptycells/
---
## JsonSaveOptions.ExportEmptyCells property

يشير إلى ما إذا كان يتم تصدير الخلايا الفارغة كقيمة null.

```csharp
public bool ExportEmptyCells { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyExportEmptyCellsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء البيانات ببعض الخلايا الفارغة
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue(2.99); // B2 is intentionally left empty

            // إنشاء JsonSaveOptions مع ExportEmptyCells مضبوط على false
            JsonSaveOptions options = new JsonSaveOptions
            {
                ExportEmptyCells = false
            };

            // حفظ إلى JSON - سيتم تخطي الخلايا الفارغة
            workbook.Save("output_skip_empty.json", options);

            // تغيير ExportEmptyCells إلى true
            options.ExportEmptyCells = true;

            // حفظ مرة أخرى - سيتم تضمين الخلايا الفارغة
            workbook.Save("output_include_empty.json", options);
        }
    }
}
```

### انظر أيضًا

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


