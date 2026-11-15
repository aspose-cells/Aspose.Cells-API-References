---
title: "فئة PdfSecurityOptions"
linktitle: "PdfSecurityOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة PdfSecurityOptions. تغلف الكائن الذي يمثل pdfsecurityoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/pdfsecurityoptions/
---

## PdfSecurityOptions class

خيارات التشفير وأذونات الوصول لمستند PDF. لا يسمح PDF/A بإعدادات الأمان.

```go

type PdfSecurityOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewPdfSecurityOptions](./newpdfsecurityoptions/) | منشئ PdfSecurityOptions |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetUserPassword](./getuserpassword/) | يحصل أو يضبط كلمة مرور المستخدم المطلوبة لفتح مستند PDF المشفر. |
| [SetUserPassword](./setuserpassword/) | يحصل أو يضبط كلمة مرور المستخدم المطلوبة لفتح مستند PDF المشفر. |
| [GetOwnerPassword](./getownerpassword/) | يحصل أو يضبط كلمة مرور المالك للمستند PDF المشفر. |
| [SetOwnerPassword](./setownerpassword/) | يحصل أو يضبط كلمة مرور المالك للمستند PDF المشفر. |
| [GetPrintPermission](./getprintpermission/) | يشير إلى ما إذا كان يُسمح بطباعة المستند. |
| [SetPrintPermission](./setprintpermission/) | يشير إلى ما إذا كان يُسمح بطباعة المستند. |
| [GetModifyDocumentPermission](./getmodifydocumentpermission/) | يشير إلى ما إذا كان يُسمح بتعديل محتويات المستند عبر عمليات غير تلك التي تتحكم فيها AnnotationsPermission و FillFormsPermission و AssembleDocumentPermission. |
| [SetModifyDocumentPermission](./setmodifydocumentpermission/) | يشير إلى ما إذا كان يُسمح بتعديل محتويات المستند عبر عمليات غير تلك التي تتحكم فيها AnnotationsPermission و FillFormsPermission و AssembleDocumentPermission. |
| [GetAnnotationsPermission](./getannotationspermission/) | يشير إلى ما إذا كان يُسمح بإضافة أو تعديل التعليقات النصية، وتعبئة حقول النماذج التفاعلية. |
| [SetAnnotationsPermission](./setannotationspermission/) | يشير إلى ما إذا كان يُسمح بإضافة أو تعديل التعليقات النصية، وتعبئة حقول النماذج التفاعلية. |
| [GetFillFormsPermission](./getfillformspermission/) | يشير إلى ما إذا كان يُسمح بتعبئة حقول النماذج التفاعلية الموجودة (بما في ذلك حقول التوقيع)، حتى إذا كان ModifyDocumentPermission غير مفعّل. |
| [SetFillFormsPermission](./setfillformspermission/) | يشير إلى ما إذا كان يُسمح بتعبئة حقول النماذج التفاعلية الموجودة (بما في ذلك حقول التوقيع)، حتى إذا كان ModifyDocumentPermission غير مفعّل. |
| [GetExtractContentPermission](./getextractcontentpermission/) | يشير إلى ما إذا كان يُسمح بنسخ أو استخراج النص والرسومات من المستند عبر عمليات غير تلك التي تتحكم فيها AccessibilityExtractContent. |
| [SetExtractContentPermission](./setextractcontentpermission/) | يشير إلى ما إذا كان يُسمح بنسخ أو استخراج النص والرسومات من المستند عبر عمليات غير تلك التي تتحكم فيها AccessibilityExtractContent. |
| [GetAccessibilityExtractContent](./getaccessibilityextractcontent/) | يشير إلى ما إذا كان يُسمح باستخراج النص والرسومات (دعمًا لإمكانية الوصول للمستخدمين ذوي الإعاقات أو لأغراض أخرى). |
| [SetAccessibilityExtractContent](./setaccessibilityextractcontent/) | يشير إلى ما إذا كان يُسمح باستخراج النص والرسومات (دعمًا لإمكانية الوصول للمستخدمين ذوي الإعاقات أو لأغراض أخرى). |
| [GetAssembleDocumentPermission](./getassembledocumentpermission/) | يشير إلى ما إذا كان يُسمح بتجميع المستند (إدراج، تدوير، أو حذف صفحات وإنشاء إشارات مرجعية أو صور مصغرة)، حتى إذا كان ModifyDocumentPermission غير مفعّل. |
| [SetAssembleDocumentPermission](./setassembledocumentpermission/) | يشير إلى ما إذا كان يُسمح بتجميع المستند (إدراج، تدوير، أو حذف صفحات وإنشاء إشارات مرجعية أو صور مصغرة)، حتى إذا كان ModifyDocumentPermission غير مفعّل. |
| [GetFullQualityPrintPermission](./getfullqualityprintpermission/) | يشير إلى ما إذا كان يُسمح بطباعة المستند إلى تمثيل يمكن من خلاله إنشاء نسخة رقمية دقيقة من محتوى PDF. |
| [SetFullQualityPrintPermission](./setfullqualityprintpermission/) | يشير إلى ما إذا كان يُسمح بطباعة المستند إلى تمثيل يمكن من خلاله إنشاء نسخة رقمية دقيقة من محتوى PDF. |
