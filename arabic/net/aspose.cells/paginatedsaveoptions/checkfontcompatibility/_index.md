---
title: "PaginatedSaveOptions.CheckFontCompatibility"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PaginatedSaveOptions. تشير إلى ما إذا كان يجب فحص توافق الخط لكل حرف في النص"
type: docs
url: /ar/net/aspose.cells/paginatedsaveoptions/checkfontcompatibility/
---
## PaginatedSaveOptions.CheckFontCompatibility property

يشير إلى ما إذا كان يجب فحص توافق الخط لكل حرف في النص.

```csharp
public bool CheckFontCompatibility { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true. قد يؤدي تعطيل هذه الخاصية إلى تحسين الأداء. ولكن عندما لا يمكن استخدام الخط الافتراضي أو المحدد للنص/الحرف لتصييره، قد تظهر أحرف غير قابلة للقراءة (مثل المربعات) في ملف PDF المُولد. في مثل هذه الحالة يجب على المستخدم إبقاء هذه الخاصية كـ true حتى يتم البحث عن خط بديل واستخدامه لتصيير النص بدلاً من ذلك؛

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckFontCompatibilityDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Compatibility Test");

            // أنشئ خيارات حفظ مجزأة
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // أظهر خاصية CheckFontCompatibility
            saveOptions.CheckFontCompatibility = false; // Disable font compatibility checking
            
            // اضبط الخصائص المطلوبة الأخرى
            saveOptions.DefaultFont = "Arial";
            saveOptions.CheckWorkbookDefaultFont = true;

            // احفظ المستند باستخدام الخيارات المحددة
            workbook.Save("PaginatedSaveOptions_CheckFontCompatibility.pdf", saveOptions);
            
            Console.WriteLine("Document saved with CheckFontCompatibility = false");
        }
    }
}
```

### انظر أيضًا

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


