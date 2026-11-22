---
title: "Enum OpenDocumentFormatVersionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Ods.OpenDocumentFormatVersionType enum. نوع إصدار تنسيق المستند المفتوح"
type: docs
url: /ar/net/aspose.cells.ods/opendocumentformatversiontype/
---
## OpenDocumentFormatVersionType enumeration

نوع إصدار تنسيق المستند المفتوح.

```csharp
public enum OpenDocumentFormatVersionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | بدون صرامة. |
| Odf11 | `1` | إصدار ODF 1.1 |
| Odf12 | `2` | إصدار ODF 1.2 |
| Odf13 | `3` | إصدار ODF 1.3 |
| Odf14 | `4` | إصدار ODF 1.4 |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OpenDocumentFormatVersionTypeDemo
    {
        public static void OpenDocumentFormatVersionTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // إنشاء OdsSaveOptions وتعيين إصدار ODF
            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;

            // حفظ دفتر العمل بتنسيق ODS باستخدام إصدار ODF المحدد
            workbook.Save("OpenDocumentFormatVersionTypeExample.ods", saveOptions);

            Console.WriteLine("Workbook saved successfully with ODF version 1.2.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


