---
title: "فئة LowCodeSaveOptionsProviderOfAssembling"
linktitle: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة LowCodeSaveOptionsProviderOfAssembling. تغلف الكائن الذي يمثل lowcodesaveoptionsproviderofassembling في Go."
type: docs
weight: 200
url: /ar/go-cpp/lowcodesaveoptionsproviderofassembling/
---

## LowCodeSaveOptionsProviderOfAssembling class

تنفيذ لتوفير خيارات حفظ تقوم بحفظ الأجزاء المقسمة إلى ملفات والمسار للملف الناتج يُسمّى كما يلي (قد يحتوي على أدلة):<see cref=\"PathHeader\"/>+<see cref=\"SheetPrefix\"/>+SheetIndex(أو SheetName)+<see cref=\"SplitPartPrefix\"/>+SplitPartIndex+<see cref=\"PathTail\"/>.

```go

type LowCodeSaveOptionsProviderOfAssembling struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfAssembling](./newlowcodesaveoptionsproviderofassembling/) | البناء الافتراضي. |
| [NewLowCodeSaveOptionsProviderOfAssembling_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofassembling_abstractlowcodesaveoptionsprovider/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetPathHeader](./getpathheader/) | جزء الرأس (قبل المحتوى المضاف للورقة والجزء المقسم) من مسار الملف. |
| [SetPathHeader](./setpathheader/) | جزء الرأس (قبل المحتوى المضاف للورقة والجزء المقسم) من مسار الملف. |
| [GetPathTail](./getpathtail/) | جزء الذيل (بعد أرقام التسلسل) من مسار الملف. يجب أن يتضمن امتداد اسم الملف. |
| [SetPathTail](./setpathtail/) | جزء الذيل (بعد أرقام التسلسل) من مسار الملف. يجب أن يتضمن امتداد اسم الملف. |
| [GetUseSheetName](./getusesheetname/) | ما إذا كان يبني مسار الملف باستخدام اسم الورقة بدلاً من فهرس الورقة. القيمة الافتراضية هي false. |
| [SetUseSheetName](./setusesheetname/) | ما إذا كان يبني مسار الملف باستخدام اسم الورقة بدلاً من فهرس الورقة. القيمة الافتراضية هي false. |
| [GetSheetPrefix](./getsheetprefix/) | بادئة لفهرس ورقة العمل. |
| [SetSheetPrefix](./setsheetprefix/) | بادئة لفهرس ورقة العمل. |
| [GetSplitPartPrefix](./getsplitpartprefix/) | بادئة لفهرس الجزء المقسم. |
| [SetSplitPartPrefix](./setsplitpartprefix/) | بادئة لفهرس الجزء المقسم. |
| [GetSheetIndexOffset](./getsheetindexoffset/) | إزاحة فهرس الورقة بين ما يُستخدم في مسار الملف وقيمته الفعلية (SplitPartInfo.SheetIndex). |
| [SetSheetIndexOffset](./setsheetindexoffset/) | إزاحة فهرس الورقة بين ما يُستخدم في مسار الملف وقيمته الفعلية (SplitPartInfo.SheetIndex). |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | إزاحة فهرس الجزء المقسم بين ما يُستخدم في مسار الملف وقيمته الفعلية (SplitPartInfo.PartIndex). |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | إزاحة فهرس الجزء المقسم بين ما يُستخدم في مسار الملف وقيمته الفعلية (SplitPartInfo.PartIndex). |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | ما إذا كان يضيف فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة فقط، لن يتم إضافة فهرس الورقة (أو اسمها) والبادئة المقابلة إلى مسار الملف. |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | ما إذا كان يضيف فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة فقط، لن يتم إضافة فهرس الورقة (أو اسمها) والبادئة المقابلة إلى مسار الملف. |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | ما إذا كان يضيف فهرس الجزء المقسم إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء مقسم واحد فقط، لن يتم إضافة فهرس الجزء المقسم والبادئة المقابلة إلى مسار الملف. |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | ما إذا كان يضيف فهرس الجزء المقسم إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء مقسم واحد فقط، لن يتم إضافة فهرس الجزء المقسم والبادئة المقابلة إلى مسار الملف. |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | القالب لإنشاء نسخة من خيارات الحفظ في GetSaveOptions(SplitPartInfo). |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | القالب لإنشاء نسخة من خيارات الحفظ في GetSaveOptions(SplitPartInfo). |
| [GetSaveOptions](./getsaveoptions/) | يحصل على خيارات الحفظ التي تُستخرج منها إعدادات الإخراج للجزء المقسم الحالي. |
| [Finish](./finish/) | يطلق الموارد بعد معالجة الجزء المقسم حالياً. |
