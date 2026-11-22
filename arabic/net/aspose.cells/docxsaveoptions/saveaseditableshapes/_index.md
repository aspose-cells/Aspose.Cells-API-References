---
title: "DocxSaveOptions.SaveAsEditableShapes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocxSaveOptions. احفظ جميع كائنات الرسم كأشكال قابلة للتحرير في ملف Word حتى تتمكن من تعديلها في Word"
type: docs
url: /ar/net/aspose.cells/docxsaveoptions/saveaseditableshapes/
---
## DocxSaveOptions.SaveAsEditableShapes property

احفظ جميع كائنات الرسم كأشكال قابلة للتحرير في ملف Word، حتى يمكنك تعديلها في Word.

```csharp
public bool SaveAsEditableShapes { get; set; }
```

### ملاحظات

للمخططات فقط.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertySaveAsEditableShapesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى وإضافة بيانات نموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Editable Shapes Demo";

            try
            {
                // تهيئة DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // اعرض القيمة الافتراضية لخاصية SaveAsEditableShapes
                Console.WriteLine("Default SaveAsEditableShapes value: " + saveOptions.SaveAsEditableShapes);

                // عيّن SaveAsEditableShapes إلى true لتوضيح استخدامه
                saveOptions.SaveAsEditableShapes = true;
                Console.WriteLine("SaveAsEditableShapes set to: " + saveOptions.SaveAsEditableShapes);

                // حفظ المصنف كملف DOCX باستخدام الخيارات المكوّنة
                workbook.Save("SaveAsEditableShapesDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with SaveAsEditableShapes option.");
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


