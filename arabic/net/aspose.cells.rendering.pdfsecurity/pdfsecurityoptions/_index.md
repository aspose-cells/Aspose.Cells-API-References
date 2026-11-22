---
title: "فئة PdfSecurityOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Rendering.PdfSecurity.PdfSecurityOptions. خيارات تشفير وصلاحيات الوصول لمستند PDF. لا يسمح PDF/A بإعدادات الأمان"
type: docs
url: /ar/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/
---
## PdfSecurityOptions class

خيارات تشفير وإعدادات أذونات الوصول لمستند PDF. لا يسمح PDF/A بإعدادات الأمان.

```csharp
public class PdfSecurityOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PdfSecurityOptions](pdfsecurityoptions/)() | المُنشئ لـ PdfSecurityOptions |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AccessibilityExtractContent](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/) { get; set; } | يُشير إلى ما إذا كان يُسمح باستخراج النصوص والرسومات (دعمًا لإمكانية الوصول للمستخدمين ذوي الإعاقة أو لأغراض أخرى). |
| [AnnotationsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/) { get; set; } | يُشير إلى ما إذا كان يُسمح بإضافة أو تعديل التعليقات النصية، وملء حقول النماذج التفاعلية. |
| [AssembleDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/) { get; set; } | يُشير إلى ما إذا كان يُسمح بتجميع المستند (إدراج، تدوير، أو حذف الصفحات وإنشاء إشارات مرجعية أو صور مصغرة)، حتى إذا كان [`ModifyDocumentPermission`](./modifydocumentpermission/) واضحًا. |
| [ExtractContentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/) { get; set; } | يُشير إلى ما إذا كان يُسمح بنسخ أو استخراج النصوص والرسومات من المستند بطرق غير تلك التي يتحكم فيها [`AccessibilityExtractContent`](./accessibilityextractcontent/). |
| [ExtractContentPermissionObsolete](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/) { get; set; } | (**Obsolete.**) الإذن بنسخ أو استخراج المحتوى تم إهماله وفقًا لمرجع PDF. |
| [FillFormsPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/) { get; set; } | يُشير إلى ما إذا كان يُسمح بملء حقول النماذج التفاعلية الموجودة (بما في ذلك حقول التوقيع)، حتى إذا كان [`ModifyDocumentPermission`](./modifydocumentpermission/) واضحًا. |
| [FullQualityPrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/) { get; set; } | يُشير إلى ما إذا كان يُسمح بطباعة المستند إلى تمثيل يمكن من خلاله إنشاء نسخة رقمية دقيقة من محتوى PDF. |
| [ModifyDocumentPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/) { get; set; } | يُشير إلى ما إذا كان يُسمح بتعديل محتويات المستند بعمليات غير تلك التي يتحكم فيها [`AnnotationsPermission`](./annotationspermission/)، [`FillFormsPermission`](./fillformspermission/) و[`AssembleDocumentPermission`](./assembledocumentpermission/). |
| [OwnerPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/) { get; set; } | يحصل أو يعيّن كلمة مرور المالك للمستند PDF المشفر. |
| [PrintPermission](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/) { get; set; } | يُشير إلى ما إذا كان يُسمح بطباعة المستند. |
| [UserPassword](../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/) { get; set; } | يحصل أو يعيّن كلمة مرور المستخدم المطلوبة لفتح المستند PDF المشفر. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Rendering.PdfSecurity;
    using System;

    public class PdfSecurityOptionsDemo
    {
        public static void PdfSecurityOptionsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Aspose";

            // إنشاء PdfSaveOptions
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // إنشاء PdfSecurityOptions
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            // تعيين خيارات الأمان
            pdfSecurityOptions.OwnerPassword = "YourOwnerPassword";
            pdfSecurityOptions.UserPassword = "YourUserPassword";
            pdfSecurityOptions.PrintPermission = true;
            pdfSecurityOptions.ModifyDocumentPermission = false;
            pdfSecurityOptions.ExtractContentPermissionObsolete = false;
            pdfSecurityOptions.AnnotationsPermission = true;
            pdfSecurityOptions.FillFormsPermission = true;
            pdfSecurityOptions.ExtractContentPermission = false;
            pdfSecurityOptions.AccessibilityExtractContent = true;
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.FullQualityPrintPermission = true;

            // تعيين خيارات الأمان إلى PdfSaveOptions
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

            // حفظ دفتر العمل كملف PDF مع خيارات الأمان المحددة
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering.PdfSecurity](../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../)


