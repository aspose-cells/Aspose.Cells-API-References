---
title: "OdsSaveOptions.OdfStrictVersion"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsSaveOptions. تحصل وتضبط نسخة ODF"
type: docs
url: /ar/net/aspose.cells/odssaveoptions/odfstrictversion/
---
## OdsSaveOptions.OdfStrictVersion property

يحصل على ويضبط إصدار ODF.

```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyOdfStrictVersionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ODF Version Demo");

            // إنشاء خيارات حفظ ODS
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            
            // ضبط نسخة ODF إلى 1.2
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // حفظ باستخدام نسخة ODF المحددة
            workbook.Save("OdfVersion12.ods", saveOptions);

            // التغيير إلى نسخة ODF 1.3
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf13;
            workbook.Save("OdfVersion13.ods", saveOptions);
        }
    }
}
```

### انظر أيضًا

* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


