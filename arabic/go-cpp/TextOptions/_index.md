---
title: "TextOptions فئة"
linktitle: "TextOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة TextOptions. تغلف الكائن الذي يمثل textoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/textoptions/
---

## TextOptions class

يمثل خيارات النص.

```go

type TextOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewTextOptions](./newtextoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetName](./getname/) | يحصل على اسم الشكل ويضبطه. |
| [SetName](./setname/) | يحصل على اسم الشكل ويضبطه. |
| [GetLanguageCode](./getlanguagecode/) | يسترجع ويضبط لغة واجهة المستخدم. |
| [SetLanguageCode](./setlanguagecode/) | يسترجع ويضبط لغة واجهة المستخدم. |
| [GetLatinName](./getlatinname/) | يسترجع ويضبط الاسم اللاتيني. |
| [SetLatinName](./setlatinname/) | يسترجع ويضبط الاسم اللاتيني. |
| [GetFarEastName](./getfareastname/) | يسترجع ويضبط اسم FarEast. |
| [SetFarEastName](./setfareastname/) | يسترجع ويضبط اسم FarEast. |
| [GetFill](./getfill/) | يمثل تنسيق التعبئة للنص. |
| [GetOutline](./getoutline/) | يمثل تنسيق المخطط للنص. |
| [GetShadow](./getshadow/) | يمثل كائن ShadowEffect الذي يحدد تأثير الظل لعنصر المخطط أو الشكل. |
| [GetUnderlineColor](./getunderlinecolor/) | يسترجع أو يضبط لون التسطير. |
| [SetUnderlineColor](./setunderlinecolor/) | يسترجع أو يضبط لون التسطير. |
| [GetKerning](./getkerning/) | يحدد الحد الأدنى لحجم الخط الذي يحدث عنده تقليل الفجوة بين الأحرف لهذا المقطع النصي. |
| [SetKerning](./setkerning/) | يحدد الحد الأدنى لحجم الخط الذي يحدث عنده تقليل الفجوة بين الأحرف لهذا المقطع النصي. |
| [GetSpacing](./getspacing/) | يحدد التباعد بين الأحرف داخل المقطع النصي. |
| [SetSpacing](./setspacing/) | يحدد التباعد بين الأحرف داخل المقطع النصي. |
| [IsNormalizeHeights](./isnormalizeheights/) | يشير إلى ما إذا كان تطبيع الارتفاع سيُطبق على المقطع النصي. |
| [SetIsNormalizeHeights](./setisnormalizeheights/) | يشير إلى ما إذا كان تطبيع الارتفاع سيُطبق على المقطع النصي. |
| [GetCapsType](./getcapstype/) | يحصل على ويضبط نوع الحروف الكبيرة للنصوص في الشكل. |
| [SetCapsType](./setcapstype/) | يحصل على ويضبط نوع الحروف الكبيرة للنصوص في الشكل. |
| [GetCharset](./getcharset/) | تمثيل مجموعة الأحرف. |
| [SetCharset](./setcharset/) | تمثيل مجموعة الأحرف. |
| [IsItalic](./isitalic/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان الخط مائلًا. |
| [SetIsItalic](./setisitalic/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان الخط مائلًا. |
| [IsBold](./isbold/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان الخط عريضًا. |
| [SetIsBold](./setisbold/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان الخط عريضًا. |
| [GetStrikeType](./getstriketype/) | يحصل على نوع الشطب للنص. |
| [SetStrikeType](./setstriketype/) | يحصل على نوع الشطب للنص. |
| [IsStrikeout](./isstrikeout/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان الخط مشطوبًا مرة واحدة. |
| [SetIsStrikeout](./setisstrikeout/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان الخط مشطوبًا مرة واحدة. |
| [GetScriptOffset](./getscriptoffset/) | يحصل ويضبط إزاحة النص، بوحدة النسبة المئوية. |
| [SetScriptOffset](./setscriptoffset/) | يحصل ويضبط إزاحة النص، بوحدة النسبة المئوية. |
| [IsSuperscript](./issuperscript/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان الخط مرتفعًا فوق السطر. |
| [SetIsSuperscript](./setissuperscript/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان الخط مرتفعًا فوق السطر. |
| [IsSubscript](./issubscript/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان الخط منخفضًا تحت السطر. |
| [SetIsSubscript](./setissubscript/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان الخط منخفضًا تحت السطر. |
| [GetUnderline](./getunderline/) | يحصل أو يضبط نوع تسطير الخط. |
| [SetUnderline](./setunderline/) | يحصل أو يضبط نوع تسطير الخط. |
| [GetDoubleSize](./getdoublesize/) | يحصل ويضبط الحجم المزدوج للخط. |
| [SetDoubleSize](./setdoublesize/) | يحصل ويضبط الحجم المزدوج للخط. |
| [GetSize](./getsize/) | يحصل أو يضبط حجم الخط. |
| [SetSize](./setsize/) | يحصل أو يضبط حجم الخط. |
| [GetThemeColor](./getthemecolor/) | يحصل ويضبط لون السمة. |
| [SetThemeColor](./setthemecolor/) | يحصل ويضبط لون السمة. |
| [GetColor](./getcolor/) | يحصل أو يضبط لون الخط. |
| [SetColor](./setcolor/) | يحصل أو يضبط لون الخط. |
| [GetArgbColor](./getargbcolor/) | يحصل ويضبط اللون باستخدام قيمة ARGB 32-بت. |
| [SetArgbColor](./setargbcolor/) | يحصل ويضبط اللون باستخدام قيمة ARGB 32-بت. |
| [Equals](./equals/) | يتحقق مما إذا كان الخطان متساويين. |
| [GetSchemeType](./getschemetype/) | يحصل ويضبط نوع النمط للخط. |
| [SetSchemeType](./setschemetype/) | يحصل ويضبط نوع النمط للخط. |
| [ToString](./tostring/) | يرجع سلسلة تمثل كائن الخلية الحالي. |
