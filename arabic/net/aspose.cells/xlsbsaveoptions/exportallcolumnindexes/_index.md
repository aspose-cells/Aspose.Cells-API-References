---
title: "XlsbSaveOptions.ExportAllColumnIndexes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية XlsbSaveOptions. تشير إلى ما إذا كان يتم تصدير جميع فهارس الأعمدة للخلايا"
type: docs
url: /ar/net/aspose.cells/xlsbsaveoptions/exportallcolumnindexes/
---
## XlsbSaveOptions.ExportAllColumnIndexes property

يشير إلى ما إذا كان يتم تصدير جميع فهارس الأعمدة للخلايا.

```csharp
public bool ExportAllColumnIndexes { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyExportAllColumnIndexesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بعض البيانات
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["C2"].PutValue(3);

            XlsbSaveOptions saveOptions = new XlsbSaveOptions
            {
                ExportAllColumnIndexes = true // Demonstrate the property usage
            };

            workbook.Save("XlsbExportAllColumnIndexes.xlsb", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


