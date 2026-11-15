---
title: "فئة FontConfigs"
linktitle: "FontConfigs"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة FontConfigs. تغلف الكائن الذي يمثل fontconfigs في Go."
type: docs
weight: 200
url: /ar/go-cpp/fontconfigs/
---

## FontConfigs class

يحدد إعدادات الخط

```go

type FontConfigs struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewFontConfigs](./newfontconfigs/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [FontConfigs_IsFontAvailable](./fontconfigs_isfontavailable/) | حدد ما إذا كان الخط متاحًا. |
| [FontConfigs_GetFontFileDataInfo](./fontconfigs_getfontfiledatainfo/) | احصل على معلومات البيانات لملف الخط. |
| [FontConfigs_GetDefaultFontName](./fontconfigs_getdefaultfontname/) | يحصل أو يعيّن اسم الخط الافتراضي. |
| [FontConfigs_SetDefaultFontName](./fontconfigs_setdefaultfontname/) | يحصل أو يعيّن اسم الخط الافتراضي. |
| [FontConfigs_GetPreferSystemFontSubstitutes](./fontconfigs_getprefersystemfontsubstitutes/) | حدد ما إذا كان يجب استخدام بدائل الخطوط النظامية أولاً أم لا عندما لا يتوفر الخط ولا يتم تعيين بديل لهذا الخط. على سبيل المثال، في Ubuntu، يتم عادة استبدال الخط "Arial" بـ "Liberation Sans". القيمة الافتراضية هي false. |
| [FontConfigs_SetPreferSystemFontSubstitutes](./fontconfigs_setprefersystemfontsubstitutes/) | حدد ما إذا كان يجب استخدام بدائل الخطوط النظامية أولاً أم لا عندما لا يتوفر الخط ولا يتم تعيين بديل لهذا الخط. على سبيل المثال، في Ubuntu، يتم عادة استبدال الخط "Arial" بـ "Liberation Sans". القيمة الافتراضية هي false. |
| [FontConfigs_SetFontSubstitutes](./fontconfigs_setfontsubstitutes/) | أسماء بدائل الخط للخط الأصلي المحدد. |
| [FontConfigs_GetFontSubstitutes](./fontconfigs_getfontsubstitutes/) | يرجع مصفوفة تحتوي على أسماء بدائل الخط لاستخدامها إذا لم يكن الخط الأصلي موجودًا. |
| [FontConfigs_SetFontFolder](./fontconfigs_setfontfolder/) | يضبط مجلد الخطوط |
| [FontConfigs_SetFontFolders](./fontconfigs_setfontfolders/) | يضبط مجلد الخطوط |
| [FontConfigs_SetFontSources](./fontconfigs_setfontsources/) | يضبط مصادر الخط. |
| [FontConfigs_GetFontSources](./fontconfigs_getfontsources/) | يحصل على نسخة من المصفوفة التي تحتوي على قائمة المصادر |
