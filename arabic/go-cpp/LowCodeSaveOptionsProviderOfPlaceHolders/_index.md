---
title: "LowCodeSaveOptionsProviderOfPlaceHolders فئة"
linktitle: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "LowCodeSaveOptionsProviderOfPlaceHolders فئة. تغلف الكائن الذي يمثل lowcodesaveoptionsproviderofplaceholders في Go."
type: docs
weight: 200
url: /ar/go-cpp/lowcodesaveoptionsproviderofplaceholders/
---

## LowCodeSaveOptionsProviderOfPlaceHolders class

تنفيذ لتوفير خيارات حفظ تقوم بحفظ الأجزاء المقسمة إلى ملفات والمسار للملف الناتج يُحدَّد باستخدام عناصر نائبة.

```go

type LowCodeSaveOptionsProviderOfPlaceHolders struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_String](./newlowcodesaveoptionsproviderofplaceholders_string/) | ينشئ نسخة لتوفير خيارات الحفظ وفقًا للقوالب المحددة. |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofplaceholders_abstractlowcodesaveoptionsprovider/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | إزاحة فهرس الورقة بين ما يُستخدم في مسار الملف وقيمته الفعلية (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | إزاحة فهرس الورقة بين ما يُستخدم في مسار الملف وقيمته الفعلية (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | إزاحة فهرس الجزء المقسم بين ما يُستخدم في مسار الملف وقيمته الفعلية (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | إزاحة فهرس الجزء المقسم بين ما يُستخدم في مسار الملف وقيمته الفعلية (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | ما إذا كان يتم إضافة فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة فقط، لن يتم إضافة فهرس الورقة والاسم والبادئة المقابلة (SheetNamePrefix) إلى مسار الملف. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | ما إذا كان يتم إضافة فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة فقط، لن يتم إضافة فهرس الورقة والاسم والبادئة المقابلة (SheetNamePrefix) إلى مسار الملف. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | ما إذا كان يتم إضافة فهرس جزء الانقسام إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء انقسام واحد فقط، لن يتم إضافة فهرس جزء الانقسام والبادئة المقابلة (SplitPartPrefix) إلى مسار الملف. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | ما إذا كان يتم إضافة فهرس جزء الانقسام إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء انقسام واحد فقط، لن يتم إضافة فهرس جزء الانقسام والبادئة المقابلة (SplitPartPrefix) إلى مسار الملف. |
| [GetSheetNamePrefix](./getsheetnameprefix/) | بادئة لفهرس ورقة العمل. |
| [SetSheetNamePrefix](./setsheetnameprefix/) | بادئة لفهرس ورقة العمل. |
| [GetSheetIndexPrefix](./getsheetindexprefix/) | بادئة لفهرس ورقة العمل. |
| [SetSheetIndexPrefix](./setsheetindexprefix/) | بادئة لفهرس ورقة العمل. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | بادئة لفهرس الجزء المقسم. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | بادئة لفهرس الجزء المقسم. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | القالب لإنشاء نسخة من خيارات الحفظ في GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | القالب لإنشاء نسخة من خيارات الحفظ في GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | يحصل على خيارات الحفظ التي تُستخرج منها إعدادات الإخراج للجزء المقسم الحالي. |
| [Finish](./finish/) | يطلق الموارد بعد معالجة الجزء المقسم حالياً. |
