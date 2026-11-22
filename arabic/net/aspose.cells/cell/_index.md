---
title: "الفئة Cell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Cell. تغلف الكائن الذي يمثل خلية واحدة في دفتر العمل."
type: docs
url: /ar/net/aspose.cells/cell/
---
## Cell class

يحتوي على الكائن الذي يمثل خلية واحدة في المصنف.

```csharp
public class Cell
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue/) { get; } | يحصل على القيمة المنطقية الموجودة في الخلية. |
| [Column](../../aspose.cells/cell/column/) { get; } | يحصل على رقم العمود (مبني على الصفر) للخلية. |
| [Comment](../../aspose.cells/cell/comment/) { get; } | يحصل على التعليق الخاص بهذه الخلية. |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink/) { get; } | يشير إلى ما إذا كانت هذه الخلية تحتوي على رابط خارجي. ينطبق فقط عندما تكون الخلية خلية صيغة. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue/) { get; } | يحصل على قيمة DateTime الموجودة في الخلية. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue/) { get; } | يحصل على قيمة السلسلة المنسقة لهذه الخلية وفقًا لنمط عرض الخلية. |
| [DoubleValue](../../aspose.cells/cell/doublevalue/) { get; } | يحصل على القيمة المزدوجة الموجودة في الخلية. |
| [EmbeddedImage](../../aspose.cells/cell/embeddedimage/) { get; set; } | يحصل على الصورة المدمجة في الخلية أو يضبطها. |
| [FloatValue](../../aspose.cells/cell/floatvalue/) { get; } | يحصل على القيمة العائمة الموجودة في الخلية. |
| [Formula](../../aspose.cells/cell/formula/) { get; set; } | يحصل على صيغة أو يضبط صيغة للـ `Cell`. |
| [FormulaLocal](../../aspose.cells/cell/formulalocal/) { get; set; } | احصل على الصيغة المنسقة حسب الإعداد المحلي للخلية. |
| [HasCustomFunction](../../aspose.cells/cell/hascustomfunction/) { get; } | يتحقق مما إذا كان هناك دالة مخصصة (دالة غير مدعومة) في صيغة هذه الخلية. |
| [HasCustomStyle](../../aspose.cells/cell/hascustomstyle/) { get; } | يشير إلى ما إذا كانت هذه الخلية لديها إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من الصف أو العمود أو دفتر العمل المقابل). |
| [HtmlString](../../aspose.cells/cell/htmlstring/) { get; set; } | يحصل على سلسلة HTML أو يضبطها التي تحتوي على بيانات وبعض التنسيقات في هذه الخلية. |
| [IntValue](../../aspose.cells/cell/intvalue/) { get; } | يحصل على القيمة الصحيحة الموجودة في الخلية. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula/) { get; } | يشير إلى ما إذا كانت صيغة الخلية صيغة مصفوفة. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader/) { get; } | يشير إلى أن صيغة الخلية هي صيغة مصفوفة وأنها الخلية الأولى في المصفوفة. |
| [IsCheckBoxStyle](../../aspose.cells/cell/ischeckboxstyle/) { get; set; } | يشير إلى ما إذا كان يتم تعيين هذه الخلية كمربع اختيار. |
| [IsDynamicArrayFormula](../../aspose.cells/cell/isdynamicarrayformula/) { get; } | يشير إلى ما إذا كانت صيغة الخلية هي صيغة مصفوفة ديناميكية (true) أو صيغة مصفوفة قديمة (false). |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue/) { get; } | يتحقق مما إذا كانت قيمة هذه الخلية خطأ. |
| [IsFormula](../../aspose.cells/cell/isformula/) { get; } | يمثل ما إذا كانت الخلية المحددة تحتوي على صيغة. |
| [IsInArray](../../aspose.cells/cell/isinarray/) { get; } | (**Obsolete.**) يشير إلى ما إذا كانت صيغة الخلية هي صيغة مصفوفة. |
| [IsInTable](../../aspose.cells/cell/isintable/) { get; } | (**Obsolete.**) يشير إلى ما إذا كانت هذه الخلية جزءًا من صيغة جدول. |
| [IsMerged](../../aspose.cells/cell/ismerged/) { get; } | يتحقق مما إذا كانت الخلية جزءًا من نطاق مدمج أم لا. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue/) { get; } | يشير إلى ما إذا كانت قيمة هذه الخلية عددية (int, double و datetime) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula/) { get; } | يشير إلى ما إذا كانت صيغة الخلية جزءًا من صيغة مشتركة. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset/) { get; } | يشير إلى ما إذا تم تعيين نمط الخلية. إذا تم إرجاع false، فهذا يعني أن هذه الخلية لديها تنسيق خلية افتراضي. |
| [IsTableFormula](../../aspose.cells/cell/istableformula/) { get; } | يشير إلى ما إذا كانت هذه الخلية جزءًا من صيغة جدول. |
| [Name](../../aspose.cells/cell/name/) { get; } | يحصل على اسم الخلية. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype/) { get; } | يمثل نوع الفئة لتنسيق الأرقام في هذه الخلية. |
| [Picture](../../aspose.cells/cell/picture/) { get; } | يحصل على كائن [`Picture`](../../aspose.cells.drawing/picture/) لتمثيل الصورة المضمنة في هذه الخلية أو null إذا لم تكن هناك صورة مدمجة لهذه الخلية. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula/) { get; set; } | يحصل أو يضبط صيغة R1C1 للـ `Cell`. |
| [Row](../../aspose.cells/cell/row/) { get; } | يحصل على رقم الصف (مبني على الصفر) للخلية. |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex/) { get; } | يحصل على فهرس النمط المشترك للخلية في مجموعة الأنماط. |
| [StringValue](../../aspose.cells/cell/stringvalue/) { get; } | يحصل على القيمة النصية الموجودة في الخلية. إذا كان نوع هذه الخلية هو نص، فسيتم إرجاع القيمة النصية نفسها. بالنسبة لأنواع الخلايا الأخرى، سيتم إرجاع القيمة النصية المُنسقة (المُنسقة باستخدام النمط المحدد لهذه الخلية). القيمة النصية المُنسقة للخلية هي نفسها ما يمكنك الحصول عليه من Excel عند نسخ خلية كنص (مثل نسخ الخلية إلى محرر نصوص أو تصدير إلى CSV). |
| [StringValueWithoutFormat](../../aspose.cells/cell/stringvaluewithoutformat/) { get; } | (**Obsolete.**) يحصل على قيمة الخلية كنص دون أي تنسيق. |
| [Type](../../aspose.cells/cell/type/) { get; } | يمثل نوع قيمة الخلية. |
| [Value](../../aspose.cells/cell/value/) { get; set; } | يحصل/يضبط القيمة الموجودة في هذه الخلية. |
| [Worksheet](../../aspose.cells/cell/worksheet/) { get; } | يحصل على ورقة العمل الأم. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate/)(CalculationOptions) | يحسب صيغة الخلية. |
| [Characters](../../aspose.cells/cell/characters/)(int, int) | يرجع كائن Characters الذي يمثل نطاقًا من الأحرف داخل نص الخلية. |
| [Copy](../../aspose.cells/cell/copy/)(Cell) | ينسخ البيانات من خلية المصدر. |
| [Equals](../../aspose.cells/cell/equals/#equals)(Cell) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع كائن خلية آخر. |
| override [Equals](../../aspose.cells/cell/equals/#equals_1)(object) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع آخر. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange/)() | يحصل على نطاق المصفوفة إذا كانت صيغة الخلية صيغة مصفوفة. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters)() | يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص الخلية. |
| [GetCharacters](../../aspose.cells/cell/getcharacters/#getcharacters_1)(bool) | يرجع جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل نص الخلية. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult/)() | احصل على نتيجة التنسيق الشرطي. |
| [GetDependents](../../aspose.cells/cell/getdependents/)(bool) | احصل على جميع الخلايا التي تشير صيغتها إلى هذه الخلية مباشرةً. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation/)(bool) | يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على هذه الخلية. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle)() | يحصل على نمط العرض لهذه الخلية. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_2)(bool) | يحصل على نمط العرض لهذه الخلية. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle/#getdisplaystyle_1)(BorderType) | يحصل على نمط العرض لهذه الخلية. |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions/)() | يحصل على شروط التنسيق التي تُطبق على هذه الخلية. |
| [GetFormula](../../aspose.cells/cell/getformula/)(bool, bool) | احصل على صيغة هذه الخلية. |
| override [GetHashCode](../../aspose.cells/cell/gethashcode/)() | يعمل كدالة تجزئة لنوع معين. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue/)() | يحصل على ارتفاع القيمة بوحدة البكسل. |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring/)(bool) | يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs)() | (**Obsolete.**) احصل على جميع الخلايا التي تشير إلى هذه الخلية مباشرةً وتحتاج إلى تحديث عندما يتم تعديل هذه الخلية. |
| [GetLeafs](../../aspose.cells/cell/getleafs/#getleafs_1)(bool) | (**Obsolete.**) احصل على جميع الخلايا التي سيتم تحديثها عندما يتم تعديل هذه الخلية. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange/)() | يرجع كائن [`Range`](../range/) الذي يمثل نطاقًا مدمجًا. |
| [GetPrecedents](../../aspose.cells/cell/getprecedents/)() | يحصل على جميع المراجع التي تظهر في صيغة هذه الخلية. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation/)() | يحصل على جميع السلف (مرجع إلى خلايا في المصنف الحالي) التي تستخدمها صيغة هذه الخلية أثناء حسابها. |
| [GetRichValue](../../aspose.cells/cell/getrichvalue/)() | يحصل على القيمة الغنية للخلية. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue/)(CellValueFormatStrategy) | يحصل على قيمة السلسلة باستخدام استراتيجية تنسيق محددة. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle)() | يحصل على نمط الخلية. |
| [GetStyle](../../aspose.cells/cell/getstyle/#getstyle_1)(bool) | إذا كان checkBorders صحيحًا، تحقق مما إذا كانت حدود الخلايا الأخرى ستؤثر على نمط هذه الخلية. |
| [GetTable](../../aspose.cells/cell/gettable/)() | يحصل على الجدول الذي يحتوي على هذه الخلية. |
| [GetValidation](../../aspose.cells/cell/getvalidation/)() | يحصل على التحقق من الصحة المطبق على هذه الخلية. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue/)() | يحصل على قيمة التحقق التي تم تطبيقها على هذه الخلية. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue/)() | يحصل على عرض القيمة بوحدة البكسل. |
| [InsertText](../../aspose.cells/cell/inserttext/)(int, string) | إدراج بعض الأحرف إلى الخلية. إذا كانت الخلية منسقة بنص غني، يمكن لهذه الطريقة الحفاظ على التنسيق الأصلي. |
| [IsRichText](../../aspose.cells/cell/isrichtext/)() | يشير إلى ما إذا كانت قيمة السلسلة لهذه الخلية نصًا منسقًا بنص غني. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue)(bool) | يضع قيمة منطقية في الخلية. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_3)(DateTime) | يضع قيمة تاريخ/وقت في الخلية. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_1)(double) | يضع قيمة مزدوجة في الخلية. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_2)(int) | يضع قيمة عددية صحيحة في الخلية. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_4)(object) | يضع قيمة كائن في الخلية. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_5)(string) | يضع قيمة سلسلة في الخلية. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_6)(string, bool) | يضع قيمة سلسلة في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان ذلك مناسبًا. |
| [PutValue](../../aspose.cells/cell/putvalue/#putvalue_7)(string, bool, bool) | يضع قيمة في الخلية، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الأرقام للخلية. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula/)(bool) | إزالة صيغة المصفوفة. |
| [Replace](../../aspose.cells/cell/replace/)(string, string, ReplaceOptions) | استبدال نص الخلية باستخدام الخيارات. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula)(string, int, int) | يضبط صيغة مصفوفة (صيغة مصفوفة قديمة تُدخل عبر CTRL+SHIFT+ENTER في مايكروسوفت إكسل) لنطاق من الخلايا. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_1)(string, int, int, FormulaParseOptions) | يضبط صيغة مصفوفة لنطاق من الخلايا. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_3)(string, int, int, bool, bool) | (**Obsolete.**) يضبط صيغة مصفوفة لنطاق من الخلايا. |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula/#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | يضبط صيغة مصفوفة لنطاق من الخلايا. |
| [SetCharacters](../../aspose.cells/cell/setcharacters/)(FontSetting[]) | يضبط تنسيق النص الغني للخلية. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula)(string, FormulaParseOptions, bool) | يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula/#setdynamicarrayformula_2)(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) | يضبط صيغة مصفوفة ديناميكية ويجعل الصيغة تمتد إلى الخلايا المجاورة إذا كان ذلك ممكنًا. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula)(string, FormulaParseOptions) | يضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_3)(string, object) | يضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_1)(string, FormulaParseOptions, object) | يضبط الصيغة والقيمة (النتيجة المحسوبة) للصيغة. |
| [SetFormula](../../aspose.cells/cell/setformula/#setformula_2)(string, bool, bool, object) | (**Obsolete.**) يضبط الصيغة والقيمة للصيغة. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula)(string, int, int) | يضبط صيغًا مشتركة لنطاق من الخلايا. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_1)(string, int, int, FormulaParseOptions) | يضبط صيغًا مشتركة لنطاق من الخلايا. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_3)(string, int, int, bool, bool) | (**Obsolete.**) يضبط صيغة لنطاق من الخلايا. |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula/#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | يضبط صيغًا مشتركة لنطاق من الخلايا. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle)(Style) | يضبط نمط الخلية. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_2)(Style, bool) | تطبيق الخاصية المعدلة للنمط على الخلية. |
| [SetStyle](../../aspose.cells/cell/setstyle/#setstyle_1)(Style, StyleFlag) | تطبيق نمط الخلية بناءً على العلامات. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_2)(int, int, string, bool, object[][]) | إنشاء جدول بيانات بمتغير واحد للنطاق المحدد بدءًا من هذه الخلية. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_3)(int, int, string, string, object[][]) | إنشاء جدول بيانات بمتغيرين للنطاق المحدد بدءًا من هذه الخلية. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula)(int, int, int, int, bool, object[][]) | إنشاء جدول بيانات بمتغير واحد للنطاق المحدد بدءًا من هذه الخلية. |
| [SetTableFormula](../../aspose.cells/cell/settableformula/#settableformula_1)(int, int, int, int, int, int, object[][]) | إنشاء جدول بيانات بمتغيرين للنطاق المحدد بدءًا من هذه الخلية. |
| [ToJson](../../aspose.cells/cell/tojson/)() | تحويل `Cell` إلى بيانات بنية JSON. |
| override [ToString](../../aspose.cells/cell/tostring/)() | إرجاع سلسلة تمثل كائن Cell الحالي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellDemo
    {
        public static void CellExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            // الوصول إلى مجموعة الخلايا
            Cells cells = worksheet.Cells;

            // وضع سلسلة نصية في خلية
            Cell cell = cells[0, 0];
            cell.PutValue("Hello");

            // وضع عدد صحيح في خلية
            cell = cells["B1"];
            cell.PutValue(12);

            // وضع عدد مزدوج في خلية
            cell = cells[0, 2];
            cell.PutValue(-1.234);

            // وضع صيغة في خلية
            cell = cells["D1"];
            cell.Formula = "=B1 + C1";

            // وضع صيغة مركبة: "sum(average(b1,c1), b1)" في الخلية b2
            cell = cells["B2"];
            cell.Formula = "=sum(average(b1,c1), b1)";

            // تعيين نمط خلية
            Style style = cell.GetStyle();
            // تعيين لون الخلفية
            style.BackgroundColor = System.Drawing.Color.Yellow;
            // تعيين خط الخلية
            style.Font.Name = "Courier New";
            style.VerticalAlignment = TextAlignmentType.Top;
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("CellExample.xlsx");
            workbook.Save("CellExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


