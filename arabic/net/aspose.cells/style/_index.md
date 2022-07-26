---
title: Style
second_title: Aspose.Cells لمرجع .NET API
description: يمثل نمط عرض مستند Excel  مثل الخط واللون والمحاذاة والحدود وما إلى ذلك . يحتوي كائن النمط على جميع سمات النمط الخط وتنسيق الأرقام والمحاذاة وما إلى ذلك كخصائص.
type: docs
weight: 5750
url: /ar/net/aspose.cells/style/
---
## Style class

يمثل نمط عرض مستند Excel ، مثل الخط واللون والمحاذاة والحدود وما إلى ذلك . يحتوي كائن النمط على جميع سمات النمط (الخط وتنسيق الأرقام والمحاذاة وما إلى ذلك) كخصائص.

```csharp
public class Style
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor) { get; set; } | الحصول على لون الخلفية وتعيينه بقيمة ARGB 32 بت. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor) { get; set; } | الحصول على لون خلفية النمط أو تعيينه . |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor) { get; set; } | الحصول على لون سمة الخلفية وتعيينه. |
| [Borders](../../aspose.cells/style/borders) { get; } | يحصل على ملف[`BorderCollection`](../bordercollection) من الاسلوب . |
| [CultureCustom](../../aspose.cells/style/culturecustom) { get; set; } | الحصول على سلسلة النمط المعتمدة على الثقافة وتعيينها لتنسيق الأرقام . إذا لم يتم تعيين تنسيق رقم لهذا الكائن ، فسيتم إرجاع قيمة فارغة. |
| [Custom](../../aspose.cells/style/custom) { get; set; } | يمثل سلسلة تنسيق الأرقام المخصصة لكائن النمط هذا. إذا لم يتم تعيين تنسيق الأرقام المخصص (على سبيل المثال ، تنسيق الأرقام مدمج) ، فسيتم إرجاع "" . |
| [Font](../../aspose.cells/style/font) { get; } | يحصل على أ[`Font`](./font) الكائن . |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor) { get; set; } | الحصول على اللون الأمامي وتعيينه بقيمة ARGB 32 بت. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor) { get; set; } | الحصول على اللون الأمامي للنمط أو تعيينه . |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor) { get; set; } | الحصول على لون المظهر الأمامي وتعيينه. |
| [HasBorders](../../aspose.cells/style/hasborders) { get; } | للتحقق مما إذا كان قد تم تعيين حدود للنمط. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment) { get; set; } | الحصول على نوع المحاذاة الأفقية للنص في الخلية أو تعيينه. |
| [IndentLevel](../../aspose.cells/style/indentlevel) { get; set; } | يمثل مستوى المسافة البادئة للخلية أو النطاق. يمكن أن يكون عددًا صحيحًا فقط من 0 إلى 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom) { get; } | الحصول على سلسلة النمط المستقل للثقافة لتنسيق الأرقام . إذا لم يتم تعيين تنسيق رقم لهذا الكائن ، فسيتم إرجاع قيمة فارغة. |
| [IsDateTime](../../aspose.cells/style/isdatetime) { get; } | يشير إلى ما إذا كان تنسيق الأرقام هو تنسيق تاريخ. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden) { get; set; } | يمثل ما إذا كانت الصيغة ستكون مخفية عندما تكون ورقة العمل محمية. |
| [IsGradient](../../aspose.cells/style/isgradient) { get; set; } | يشير إلى ما إذا كان تظليل الخلية عبارة عن نمط متدرج. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed) { get; set; } | يشير إلى ما إذا كان يجب استخدام المحاذاة الموزعة أو المضبوطة للخلايا في السطر الأخير من النص. |
| [IsLocked](../../aspose.cells/style/islocked) { get; set; } | الحصول على أو تعيين قيمة تشير إلى إمكانية تعديل الخلية أم لا. |
| [IsPercent](../../aspose.cells/style/ispercent) { get; } | يشير إلى ما إذا كان تنسيق الأرقام هو تنسيق النسبة المئوية. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان النص داخل الخلية ملتفًا أم لا. |
| [Name](../../aspose.cells/style/name) { get; set; } | الحصول على اسم النمط أو تحديده. |
| [Number](../../aspose.cells/style/number) { get; set; } | الحصول على تنسيق عرض الأرقام والتواريخ أو تحديده. تختلف أنماط التنسيق باختلاف المناطق. |
| [ParentStyle](../../aspose.cells/style/parentstyle) { get; } | الحصول على النمط الأصل لهذا النمط . |
| [Pattern](../../aspose.cells/style/pattern) { get; set; } | الحصول على نوع نمط خلفية الخلية أو تعيينه. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix) { get; set; } | يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة. |
| [RotationAngle](../../aspose.cells/style/rotationangle) { get; set; } | يمثل زاوية دوران النص. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit) { get; set; } | يمثل حالة تقلص النص تلقائيًا ليلائم عرض العمود المتاح. |
| [TextDirection](../../aspose.cells/style/textdirection) { get; set; } | يمثل ترتيب قراءة النص. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment) { get; set; } | الحصول على نوع المحاذاة الرأسية للنص في الخلية أو تعيينه. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Copy](../../aspose.cells/style/copy)(Style) | نسخ البيانات من كائن نمط آخر |
| override [Equals](../../aspose.cells/style/equals)(object) | تحديد ما إذا كان مثيلا النمط متساويين. |
| override [GetHashCode](../../aspose.cells/style/gethashcode)() | تعمل كدالة تجزئة لكائن نمط. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient)(out Color, out Color, out GradientStyleType, out int) | احصل على إعداد التدرج ثنائي اللون. |
| [IsModified](../../aspose.cells/style/ismodified)(StyleModifyFlag) | للتحقق مما إذا كانت الخصائص المحددة للنمط قد تم تعديلها. يُستخدم لنمط التنسيقات الشرطية للتحقق مما إذا كان يجب استخدام الخصائص المحددة لهذا النمط عند تطبيق التنسيقات الشرطية على خلية. |
| [SetBorder](../../aspose.cells/style/setborder)(BorderType, CellBorderType, Color) | يعين حدود النمط . |
| [SetCustom](../../aspose.cells/style/setcustom)(string, bool) | يعين سلسلة تنسيق الأرقام المخصص لخلية. |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor)(BackgroundType, Color, Color) | يضبط لون الخلفية. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient)(Color, Color, GradientStyleType, int) | يضبط التعبئة المحددة لتدرج لوني ثنائي اللون. |
| [Update](../../aspose.cells/style/update)() | قم بتطبيق النمط المسمى على أنماط الخلايا التي تستخدم هذا النمط المسمى. إنه يعمل مثل النقر فوق الزر "موافق" بعد الانتهاء من تعديل النمط. ينطبق فقط على النمط المسمى. |

### أمثلة

```csharp
[C#]
Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;
Cell cell = sheets[0].Cells["A1"];
Style style =  cell.GetStyle();
style.Font.Name = "Times New Roman";
style.Font.Color = Color.Blue;
cell.SetStyle(style);
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
