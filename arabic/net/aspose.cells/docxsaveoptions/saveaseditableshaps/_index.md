---
title: "DocxSaveOptions.SaveAsEditableShaps"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocxSaveOptions. احفظ جميع كائنات الرسم كأشكال قابلة للتحرير في ملف Word. بحيث يمكنك تعديلها في Word"
type: docs
url: /ar/net/aspose.cells/docxsaveoptions/saveaseditableshaps/
---
## DocxSaveOptions.SaveAsEditableShaps property

احفظ جميع كائنات الرسم كأشكال قابلة للتحرير في ملف Word. بحيث يمكنك تعديلها في Word.

```csharp
[Obsolete("Use SaveFormat.SaveAsEditableShapes instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SaveAsEditableShaps { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية [`SaveAsEditableShapes`](../saveaseditableshapes/) . سيتم إزالة هذه الخاصية بعد 6 أشهر منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveAsEditableShapsDemo
    {
        public static void Run()
        {
            // أنشئ كائن مصنف وافتح ملف Excel القالب
            Workbook workbook = new Workbook("example.xlsx");

            // تهيئة DocxSaveOptions
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            
            // عيّن خاصية SaveAsEditableShaps إلى true
            saveOptions.SaveAsEditableShaps = true;

            // احفظ المصنف كـ DOCX باستخدام الخيارات المحددة
            workbook.Save("example.docx", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


