---
title: "تعداد OoxmlCompressionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.OoxmlCompressionType. نوع ضغط Ooxml"
type: docs
url: /ar/net/aspose.cells/ooxmlcompressiontype/
---
## OoxmlCompressionType enumeration

نوع ضغط Ooxml

```csharp
public enum OoxmlCompressionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Level1 | `1` | أسرع ضغط لكنه الأقل فاعلية. |
| Level2 | `2` | أبطأ قليلاً، ولكن أفضل، من المستوى 1. |
| Level3 | `3` | أبطأ قليلاً، ولكن أفضل، من المستوى 2. |
| Level4 | `4` | أبطأ قليلاً، ولكن أفضل، من المستوى 3. |
| Level5 | `5` | أبطأ قليلاً من المستوى 4، ولكن مع ضغط أفضل. |
| Level6 | `6` | توازن جيد بين السرعة وكفاءة الضغط. |
| Level7 | `7` | ضغط جيد جداً! |
| Level8 | `8` | ضغط أفضل من المستوى 7! |
| Level9 | `9` | ضغط "الأفضل"، حيث يعني الأفضل أكبر تقليل في حجم تدفق البيانات المدخل. وهذا أيضاً أبطأ ضغط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlCompressionTypeDemo
    {
        public static void OoxmlCompressionTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // إنشاء OoxmlSaveOptions وتحديد نوع الضغط
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6; // A good balance of speed and compression efficiency

            // احفظ دفتر العمل بنوع الضغط المحدد
            workbook.Save("OoxmlCompressionTypeExample.xlsx", saveOptions);

            Console.WriteLine("Workbook saved with OoxmlCompressionType.Level6 compression.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


