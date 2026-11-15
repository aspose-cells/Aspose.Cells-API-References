---
title: "فئة Style"
linktitle: "Style"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة Style. تغلف الكائن الذي يمثل style في Go."
type: docs
weight: 200
url: /ar/go-cpp/style/
---

## Style class

يمثل نمط العرض لمستند Excel، مثل الخط، اللون، المحاذاة، الحدود، إلخ. يحتوي كائن Style على جميع سمات النمط (الخط، تنسيق الأرقام، المحاذاة، وما إلى ذلك) كخصائص.

```go

type Style struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetBackgroundThemeColor](./getbackgroundthemecolor/) | يحصل على لون سمة الخلفية ويضبطه. |
| [SetBackgroundThemeColor](./setbackgroundthemecolor/) | يحصل على لون سمة الخلفية ويضبطه. |
| [GetForegroundThemeColor](./getforegroundthemecolor/) | يحصل على لون سمة المقدمة ويضبطه. |
| [SetForegroundThemeColor](./setforegroundthemecolor/) | يحصل على لون سمة المقدمة ويضبطه. |
| [GetName](./getname/) | يحصل على اسم النمط أو يضبطه. |
| [SetName](./setname/) | يحصل على اسم النمط أو يضبطه. |
| [GetPattern](./getpattern/) | يحصل على نوع نمط خلفية الخلية أو يضبطه. |
| [SetPattern](./setpattern/) | يحصل على نوع نمط خلفية الخلية أو يضبطه. |
| [SetPatternColor](./setpatterncolor/) | يضبط لون الخلفية. |
| [GetBorders](./getborders/) | يحصل على BorderCollection للنمط. |
| [GetBackgroundColor](./getbackgroundcolor/) | يحصل على لون خلفية النمط أو يضبطه. |
| [SetBackgroundColor](./setbackgroundcolor/) | يحصل على لون خلفية النمط أو يضبطه. |
| [GetBackgroundArgbColor](./getbackgroundargbcolor/) | يحصل على لون الخلفية ويضبطه باستخدام قيمة ARGB 32‑بت. |
| [SetBackgroundArgbColor](./setbackgroundargbcolor/) | يحصل على لون الخلفية ويضبطه باستخدام قيمة ARGB 32‑بت. |
| [GetForegroundColor](./getforegroundcolor/) | يحصل على لون مقدمة النمط أو يضبطه. |
| [SetForegroundColor](./setforegroundcolor/) | يحصل على لون مقدمة النمط أو يضبطه. |
| [GetForegroundArgbColor](./getforegroundargbcolor/) | يحصل على لون المقدمة ويضبطه باستخدام قيمة ARGB 32‑بت. |
| [SetForegroundArgbColor](./setforegroundargbcolor/) | يحصل على لون المقدمة ويضبطه باستخدام قيمة ARGB 32‑بت. |
| [Copy](./copy/) | ينسخ البيانات من كائن نمط آخر |
| [GetHasBorders](./gethasborders/) | يتحقق مما إذا تم تعيين حدود للنمط. |
| [GetParentStyle](./getparentstyle/) | يحصل على النمط الأب لهذا النمط. |
| [Update](./update/) | تطبيق النمط المسمى على أنماط الخلايا التي تستخدم هذا النمط المسمى. يعمل كما النقر على زر "موافق" بعد الانتهاء من تعديل النمط. ينطبق فقط على النمط المسمى. |
| [IsNumberFormatApplied](./isnumberformatapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق الأرقام. |
| [SetIsNumberFormatApplied](./setisnumberformatapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق الأرقام. |
| [IsFontApplied](./isfontapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق الخط. |
| [SetIsFontApplied](./setisfontapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق الخط. |
| [IsAlignmentApplied](./isalignmentapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق المحاذاة. |
| [SetIsAlignmentApplied](./setisalignmentapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق المحاذاة. |
| [IsBorderApplied](./isborderapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق الحدود. |
| [SetIsBorderApplied](./setisborderapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق الحدود. |
| [IsFillApplied](./isfillapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق التعبئة. |
| [SetIsFillApplied](./setisfillapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق التعبئة. |
| [IsProtectionApplied](./isprotectionapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق الحماية. |
| [SetIsProtectionApplied](./setisprotectionapplied/) | تحديد ما إذا كان يجب تطبيق تنسيق الحماية. |
| [IsModified](./ismodified/) | يتحقق مما إذا تم تعديل الخصائص المحددة للنمط. يُستخدم لنمط الـ ConditionalFormattings للتحقق مما إذا كان يجب استخدام الخصائص المحددة لهذا النمط عند تطبيق الـ ConditionalFormattings على خلية. |
| [Equals](./equals/) | يحدد ما إذا كان كائني Style متساويين. |
| [GetHashCode](./gethashcode/) | يعمل كدالة تجزئة لكائن Style. |
| [GetIndentLevel](./getindentlevel/) | يمثل مستوى المسافة البادئة للخلية أو النطاق. يمكن أن يكون عددًا صحيحًا فقط من 0 إلى 250. |
| [SetIndentLevel](./setindentlevel/) | يمثل مستوى المسافة البادئة للخلية أو النطاق. يمكن أن يكون عددًا صحيحًا فقط من 0 إلى 250. |
| [GetFont](./getfont/) | يحصل على كائن Font. |
| [GetRotationAngle](./getrotationangle/) | يمثل زاوية دوران النص. |
| [SetRotationAngle](./setrotationangle/) | يمثل زاوية دوران النص. |
| [GetHorizontalAlignment](./gethorizontalalignment/) | يحصل أو يضبط نوع محاذاة النص الأفقي في الخلية. |
| [SetHorizontalAlignment](./sethorizontalalignment/) | يحصل أو يضبط نوع محاذاة النص الأفقي في الخلية. |
| [GetVerticalAlignment](./getverticalalignment/) | يحصل أو يضبط نوع محاذاة النص العمودي في الخلية. |
| [SetVerticalAlignment](./setverticalalignment/) | يحصل أو يضبط نوع محاذاة النص العمودي في الخلية. |
| [IsTextWrapped](./istextwrapped/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان النص داخل الخلية ملتفًا. |
| [SetIsTextWrapped](./setistextwrapped/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان النص داخل الخلية ملتفًا. |
| [GetNumber](./getnumber/) | يحصل أو يضبط تنسيق عرض الأرقام والتواريخ. أنماط التنسيق تختلف بين المناطق. |
| [SetNumber](./setnumber/) | يحصل أو يضبط تنسيق عرض الأرقام والتواريخ. أنماط التنسيق تختلف بين المناطق. |
| [SetBorder_BorderType_CellBorderType_Color](./setborder_bordertype_cellbordertype_color/) | يضبط حدود النمط. |
| [SetBorder_BorderType_CellBorderType_CellsColor](./setborder_bordertype_cellbordertype_cellscolor/) | يضبط حدود النمط. |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | اضبط حدود المخطط الخارجي |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | اضبط حدود المخطط الخارجي |
| [IsLocked](./islocked/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا. |
| [SetIsLocked](./setislocked/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان يمكن تعديل الخلية أم لا. |
| [SetCustom_String_Bool](./setcustom_string_bool/) | يضبط سلسلة تنسيق الرقم المخصص للخلية. |
| [GetCustom](./getcustom/) | يمثل سلسلة تنسيق الرقم المخصص لهذا الكائن النمطي. إذا لم يتم تعيين تنسيق الرقم المخصص (على سبيل المثال، تنسيق الرقم مدمج)، سيتم إرجاع \"\". |
| [SetCustom_String](./setcustom_string/) | يمثل سلسلة تنسيق الرقم المخصص لهذا الكائن النمطي. إذا لم يتم تعيين تنسيق الرقم المخصص (على سبيل المثال، تنسيق الرقم مدمج)، سيتم إرجاع \"\". |
| [GetCultureCustom](./getculturecustom/) | يحصل ويضبط سلسلة النمط المعتمدة على الثقافة لتنسيق الرقم. إذا لم يتم تعيين تنسيق رقم لهذا الكائن، سيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا، سيتم إرجاع سلسلة النمط المقابلة للرقم المدمج. |
| [SetCultureCustom](./setculturecustom/) | يحصل ويضبط سلسلة النمط المعتمدة على الثقافة لتنسيق الرقم. إذا لم يتم تعيين تنسيق رقم لهذا الكائن، سيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا، سيتم إرجاع سلسلة النمط المقابلة للرقم المدمج. |
| [GetInvariantCustom](./getinvariantcustom/) | يحصل على سلسلة النمط غير المعتمدة على الثقافة لتنسيق الرقم. إذا لم يتم تعيين تنسيق رقم لهذا الكائن، سيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا، سيتم إرجاع سلسلة النمط المقابلة للرقم المدمج. |
| [IsFormulaHidden](./isformulahidden/) | يمثل ما إذا كانت الصيغة ستُخفى عندما تكون ورقة العمل محمية. |
| [SetIsFormulaHidden](./setisformulahidden/) | يمثل ما إذا كانت الصيغة ستُخفى عندما تكون ورقة العمل محمية. |
| [GetShrinkToFit](./getshrinktofit/) | يمثل ما إذا كان النص يتقلص تلقائيًا ليتناسب مع عرض العمود المتاح. |
| [SetShrinkToFit](./setshrinktofit/) | يمثل ما إذا كان النص يتقلص تلقائيًا ليتناسب مع عرض العمود المتاح. |
| [GetTextDirection](./gettextdirection/) | يمثل ترتيب قراءة النص. |
| [SetTextDirection](./settextdirection/) | يمثل ترتيب قراءة النص. |
| [IsJustifyDistributed](./isjustifydistributed/) | يشير إلى ما إذا كان يجب استخدام محاذاة مبررة أو موزعة للخلايا في السطر الأخير من النص. |
| [SetIsJustifyDistributed](./setisjustifydistributed/) | يشير إلى ما إذا كان يجب استخدام محاذاة مبررة أو موزعة للخلايا في السطر الأخير من النص. |
| [GetQuotePrefix](./getquoteprefix/) | يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة. |
| [SetQuotePrefix](./setquoteprefix/) | يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة. |
| [IsGradient](./isgradient/) | يشير إلى ما إذا كان تظليل الخلية نمطًا متدرجًا. |
| [SetIsGradient](./setisgradient/) | يشير إلى ما إذا كان تظليل الخلية نمطًا متدرجًا. |
| [SetTwoColorGradient](./settwocolorgradient/) | يضبط التعبئة المحددة لتصبح تدرجًا لونيًا من لونين. |
| [GetTwoColorGradientSetting](./gettwocolorgradientsetting/) | احصل على إعداد التدرج اللوني ثنائي اللون. |
| [IsPercent](./ispercent/) | يشير إلى ما إذا كان تنسيق الرقم هو تنسيق نسبة مئوية. |
| [IsDateTime](./isdatetime/) | يشير إلى ما إذا كان تنسيق الرقم هو تنسيق تاريخ. |
| [IsCheckBox](./ischeckbox/) | يشير إلى ما إذا كان ذلك نمطًا لمربع اختيار. |
| [SetIsCheckBox](./setischeckbox/) | يشير إلى ما إذا كان ذلك نمطًا لمربع اختيار. |
| [ToJson](./tojson/) | حوّل النمط إلى بيانات هيكل JSON. |
| [GetLeftBorder](./getleftborder/) | يحصل على الحد الأيسر. |
| [GetRightBorder](./getrightborder/) | يحصل على الحد الأيمن. |
| [GetTopBorder](./gettopborder/) | يسترجع الحد العلوي. |
| [GetBottomBorder](./getbottomborder/) | يسترجع الحد السفلي. |
