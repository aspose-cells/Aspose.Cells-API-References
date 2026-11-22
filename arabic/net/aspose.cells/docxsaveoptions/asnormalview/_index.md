---
title: "DocxSaveOptions.AsNormalView"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocxSaveOptions. تصدير ملف Excel إلى ملف docx كعرض عادي. إذا كانت هذه الخاصية true سيتم إخراج منطقة واحدة ولن يُطبق أي مقياس. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/docxsaveoptions/asnormalview/
---
## DocxSaveOptions.AsNormalView property

تصدير ملف Excel إلى ملف docx كعرض عادي. إذا كانت هذه الخاصية true ، سيتم إخراج منطقة واحدة، ولن يؤثر أي مقياس. القيمة الافتراضية هي false.

```csharp
public bool AsNormalView { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertyAsNormalViewDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى وإضافة بيانات نموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Normal View Demo";

            try
            {
                // تهيئة DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // اعرض القيمة الافتراضية لخاصية AsNormalView
                Console.WriteLine("Default AsNormalView value: " + saveOptions.AsNormalView);

                // عيّن AsNormalView إلى true لتوضيح استخدامه
                saveOptions.AsNormalView = true;
                Console.WriteLine("AsNormalView set to: " + saveOptions.AsNormalView);

                // حفظ المصنف كملف DOCX باستخدام الخيارات المكوّنة
                workbook.Save("AsNormalViewDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with AsNormalView option.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


