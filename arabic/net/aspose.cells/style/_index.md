---
title: "فئة Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Style. تمثل نمط العرض لمستندات Excel مثل لون الخط والمحاذاة والحدود وغيرها. يحتوي كائن Style على جميع سمات النمط مثل الخط وتنسيق الرقم والمحاذاة وما إلى ذلك كخصائص."
type: docs
url: /ar/net/aspose.cells/style/
---
## Style class

يمثل نمط العرض لمستند Excel، مثل الخط واللون والمحاذاة والحدود، إلخ. يحتوي كائن Style على جميع سمات النمط (الخط، تنسيق الأرقام، المحاذاة، وما إلى ذلك) كخصائص.

```csharp
public class Style
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Style](style/)() | (**Obsolete.**) يهيئ مثيلًا جديدًا من الفئة `Style`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor/) { get; set; } | يحصل على اللون الخلفي ويضبطه باستخدام قيمة ARGB 32 بت. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor/) { get; set; } | يحصل على لون الخلفية للنمط أو يضبطه. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor/) { get; set; } | يحصل على لون سمة الخلفية ويضبطه. |
| [Borders](../../aspose.cells/style/borders/) { get; } | يحصل على [`BorderCollection`](../bordercollection/) للنمط. |
| [BottomBorder](../../aspose.cells/style/bottomborder/) { get; } | يحصل على الحد السفلي. |
| [CultureCustom](../../aspose.cells/style/culturecustom/) { get; set; } | يحصل على سلسلة النمط المعتمدة على الثقافة لتنسيق الأرقام ويضبطها. إذا لم يتم تعيين تنسيق رقم لهذا الكائن، سيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا، سيتم إرجاع سلسلة النمط المقابلة للرقم المدمج. |
| [Custom](../../aspose.cells/style/custom/) { get; set; } | يمثل سلسلة تنسيق الرقم المخصص لهذا الكائن من النوع Style. إذا لم يتم تعيين تنسيق الرقم المخصص (على سبيل المثال، إذا كان تنسيق الرقم مدمجًا)، سيتم إرجاع "". |
| [Font](../../aspose.cells/style/font/) { get; } | يحصل على كائن [`Font`](./font/). |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor/) { get; set; } | يحصل على اللون الأمامي ويضبطه باستخدام قيمة ARGB 32 بت. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor/) { get; set; } | يحصل على لون الأمام للنمط أو يضبطه. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor/) { get; set; } | يحصل على لون سمة المقدمة ويضبطه. |
| [HasBorders](../../aspose.cells/style/hasborders/) { get; } | يتحقق مما إذا تم تعيين حدود للنمط. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment/) { get; set; } | يحصل على نوع محاذاة النص الأفقية في الخلية أو يضبطه. |
| [IndentLevel](../../aspose.cells/style/indentlevel/) { get; set; } | يمثل مستوى المسافة البادئة للخلية أو النطاق. يمكن أن يكون عددًا صحيحًا فقط من 0 إلى 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom/) { get; } | يحصل على سلسلة النمط المستقلة عن الثقافة لتنسيق الأرقام. إذا لم يتم تعيين تنسيق رقم لهذا الكائن، سيتم إرجاع null. إذا كان تنسيق الرقم مدمجًا، سيتم إرجاع سلسلة النمط المقابلة للرقم المدمج. |
| [IsAlignmentApplied](../../aspose.cells/style/isalignmentapplied/) { get; set; } | يشير إلى ما إذا كان يجب تطبيق تنسيق المحاذاة. |
| [IsBorderApplied](../../aspose.cells/style/isborderapplied/) { get; set; } | يشير إلى ما إذا كان يجب تطبيق تنسيق الحدود. |
| [IsCheckBox](../../aspose.cells/style/ischeckbox/) { get; set; } | يشير إلى ما إذا كان نمطًا لمربع الاختيار. |
| [IsDateTime](../../aspose.cells/style/isdatetime/) { get; } | يشير إلى ما إذا كان تنسيق الرقم هو تنسيق تاريخ. |
| [IsFillApplied](../../aspose.cells/style/isfillapplied/) { get; set; } | يشير إلى ما إذا كان يجب تطبيق تنسيق التعبئة. |
| [IsFontApplied](../../aspose.cells/style/isfontapplied/) { get; set; } | يشير إلى ما إذا كان يجب تطبيق تنسيق الخط. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden/) { get; set; } | يمثل ما إذا كانت الصيغة ستُخفى عندما يتم حماية ورقة العمل. |
| [IsGradient](../../aspose.cells/style/isgradient/) { get; set; } | يشير إلى ما إذا كان تظليل الخلية نمطًا متدرجًا. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed/) { get; set; } | يشير إلى ما إذا كان يجب استخدام محاذاة مبررة أو موزعة للخلية في السطر الأخير من النص. |
| [IsLocked](../../aspose.cells/style/islocked/) { get; set; } | يحصل على قيمة أو يضبطها تشير إلى ما إذا كان يمكن تعديل الخلية أم لا. |
| [IsNumberFormatApplied](../../aspose.cells/style/isnumberformatapplied/) { get; set; } | يشير إلى ما إذا كان يجب تطبيق تنسيق الأرقام. |
| [IsPercent](../../aspose.cells/style/ispercent/) { get; } | يشير إلى ما إذا كان تنسيق الرقم هو تنسيق نسبة مئوية. |
| [IsProtectionApplied](../../aspose.cells/style/isprotectionapplied/) { get; set; } | يشير إلى ما إذا كان يجب تطبيق تنسيق الحماية. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped/) { get; set; } | يحصل على قيمة أو يضبطها تشير إلى ما إذا كان النص داخل الخلية مُلتفًا. |
| [LeftBorder](../../aspose.cells/style/leftborder/) { get; } | يحصل على الحد الأيسر. |
| [Name](../../aspose.cells/style/name/) { get; set; } | يحصل على اسم النمط أو يضبطه. |
| [Number](../../aspose.cells/style/number/) { get; set; } | يحصل على تنسيق العرض للأرقام والتواريخ أو يضبطه. أنماط التنسيق تختلف بين المناطق المختلفة. |
| [ParentStyle](../../aspose.cells/style/parentstyle/) { get; } | يحصل على النمط الأب لهذا النمط. |
| [Pattern](../../aspose.cells/style/pattern/) { get; set; } | يحصل على نوع نمط خلفية الخلية أو يضبطه. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix/) { get; set; } | يشير إلى ما إذا كانت قيمة الخلية تبدأ بعلامة اقتباس مفردة. |
| [RightBorder](../../aspose.cells/style/rightborder/) { get; } | يحصل على الحد الأيمن. |
| [RotationAngle](../../aspose.cells/style/rotationangle/) { get; set; } | يمثل زاوية دوران النص. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit/) { get; set; } | يمثل ما إذا كان النص يتقلص تلقائيًا ليتناسب مع عرض العمود المتاح. |
| [TextDirection](../../aspose.cells/style/textdirection/) { get; set; } | يمثل ترتيب قراءة النص. |
| [TopBorder](../../aspose.cells/style/topborder/) { get; } | يحصل على الحد العلوي. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment/) { get; set; } | يحصل أو يضبط نوع المحاذاة العمودية للنص في الخلية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Copy](../../aspose.cells/style/copy/)(Style) | ينسخ البيانات من كائن نمط آخر |
| override [Equals](../../aspose.cells/style/equals/)(object) | يحدد ما إذا كان كائني Style متساويين. |
| override [GetHashCode](../../aspose.cells/style/gethashcode/)() | يعمل كدالة تجزئة لكائن Style. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient/)(out Color, out Color, out GradientStyleType, out int) | (**مهمل.**) احصل على إعداد التدرج اللوني ثنائي اللون. |
| [GetTwoColorGradientSetting](../../aspose.cells/style/gettwocolorgradientsetting/)() | احصل على إعداد التدرج اللوني ثنائي اللون. |
| [IsModified](../../aspose.cells/style/ismodified/)(StyleModifyFlag) | يتحقق مما إذا كانت الخصائص المحددة للنمط قد تم تعديلها. يُستخدم لنمط ConditionalFormattings للتحقق مما إذا كان يجب استخدام الخصائص المحددة لهذا النمط عند تطبيق ConditionalFormattings على خلية. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder)(BorderType, CellBorderType, CellsColor) | يضبط حدود النمط. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder_1)(BorderType, CellBorderType, Color) | يضبط حدود النمط. |
| [SetCustom](../../aspose.cells/style/setcustom/)(string, bool) | يضبط سلسلة تنسيق الرقم المخصص لخلية. |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | اضبط حدود المخطط الخارجي |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | اضبط حدود المخطط الخارجي |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor/)(BackgroundType, Color, Color) | يضبط لون الخلفية. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient/)(Color, Color, GradientStyleType, int) | يضبط التعبئة المحددة لتصبح تدرجًا لونيًا ثنائي اللون. |
| [ToJson](../../aspose.cells/style/tojson/)() | حوّل `Style` إلى بيانات بنية JSON. |
| [Update](../../aspose.cells/style/update/)() | طبق النمط المسمى على أنماط الخلايا التي تستخدم هذا النمط المسمى. يعمل كما لو قمت بالنقر على زر "ok" بعد الانتهاء من تعديل النمط. يُطبق فقط على النمط المسمى. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleDemo
    {
        public static void StyleExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى خلية من ورقة العمل
            Cell cell = worksheet.Cells["A1"];
            
            // احصل على نمط الخلية
            Style style = cell.GetStyle();
            
            // اضبط خصائص مختلفة للنمط
            style.Font.Name = "Times New Roman";
            style.Font.Color = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;
            style.IsLocked = true;
            style.Number = 15; // Date format
            style.IndentLevel = 2;
            style.RotationAngle = 45;
            style.IsFormulaHidden = true;
            style.ShrinkToFit = true;
            style.TextDirection = TextDirectionType.RightToLeft;
            style.IsJustifyDistributed = true;
            style.QuotePrefix = true;
            style.IsGradient = true;
            style.IsNumberFormatApplied = true;
            style.IsFontApplied = true;
            style.IsAlignmentApplied = true;
            style.IsBorderApplied = true;
            style.IsFillApplied = true;
            style.IsProtectionApplied = true;
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.ForegroundArgbColor = Color.Red.ToArgb();
            style.Custom = "0.00%";
            style.CultureCustom = "0.00%";
            
            // اضبط النمط للخلية
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("StyleExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


