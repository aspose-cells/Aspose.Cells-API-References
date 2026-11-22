---
title: "DocxSaveOptions.DocxSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ DocxSaveOptions. يمثل خيارات حفظ ملف .docx"
type: docs
url: /ar/net/aspose.cells/docxsaveoptions/docxsaveoptions/
---
## DocxSaveOptions() {#constructor}

يمثل خيارات حفظ ملف .docx.

```csharp
public DocxSaveOptions()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإضافة بيانات نموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // تهيئة DocxSaveOptions باستخدام المنشئ
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.SaveAsEditableShaps = true;
            
            // حفظ المصنف كملف DOCX مع الخيارات
            workbook.Save("output.docx", saveOptions);
            
            Console.WriteLine("Document saved successfully with DocxSaveOptions.");
        }
    }
}
```

### انظر أيضًا

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DocxSaveOptions(bool) {#constructor_1}

يمثل خيارات حفظ ملف .docx.

```csharp
public DocxSaveOptions(bool saveAsImage)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| saveAsImage | منطقي | إذا كان True، سيتم تحويل المصنف إلى بعض الصور في ملف .docx. إذا كان False، سيتم تحويل المصنف إلى بعض الجداول في ملف .docx. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // احفظ كـ DOCX باستخدام الخيارات الافتراضية
            workbook.Save("output_default.docx");
            
            // احفظ كـ DOCX باستخدام DocxSaveOptions(true) - مُحسّن لـ MS Word
            workbook.Save("output_optimized.docx", new DocxSaveOptions(true));
        }
    }
}
```

### انظر أيضًا

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


