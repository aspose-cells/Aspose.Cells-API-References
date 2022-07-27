---
title: Cell
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف الكائن الذي يمثل خلية مصنف واحدة.
type: docs
weight: 230
url: /ar/net/aspose.cells/cell/
---
## Cell class

لتغليف الكائن الذي يمثل خلية مصنف واحدة.

```csharp
public class Cell
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue) { get; } | الحصول على القيمة المنطقية الموجودة في الخلية. |
| [Column](../../aspose.cells/cell/column) { get; } | الحصول على رقم العمود (على أساس الصفر) للخلية . |
| [Comment](../../aspose.cells/cell/comment) { get; } | الحصول على تعليق هذه الخلية . |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink) { get; } | يشير إلى ما إذا كانت هذه الخلية تحتوي على ارتباط خارجي . يتم تطبيقه فقط عندما تكون الخلية عبارة عن خلية صيغة. |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue) { get; } | الحصول على قيمة DateTime الموجودة في الخلية. |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue) { get; } | الحصول على قيمة السلسلة المنسقة لهذه الخلية حسب نمط عرض الخلية. |
| [DoubleValue](../../aspose.cells/cell/doublevalue) { get; } | الحصول على القيمة المزدوجة الموجودة في الخلية. |
| [FloatValue](../../aspose.cells/cell/floatvalue) { get; } | الحصول على القيمة العائمة الموجودة في الخلية. |
| [Formula](../../aspose.cells/cell/formula) { get; set; } | الحصول على صيغة ملف[`Cell`](../cell) . |
| [FormulaLocal](../../aspose.cells/cell/formulalocal) { get; set; } | احصل على الصيغة المنسقة محليًا للخلية. |
| [HtmlString](../../aspose.cells/cell/htmlstring) { get; set; } | الحصول على وتعيين سلسلة html التي تحتوي على بيانات وبعض التنسيقات في هذه الخلية. |
| [IntValue](../../aspose.cells/cell/intvalue) { get; } | الحصول على قيمة العدد الصحيح الموجود في الخلية. |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula) { get; } | يشير إلى ما إذا كانت صيغة الخلية صيغة صفيف. |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader) { get; } | تشير إلى أن صيغة الخلية هي وصيغة الصفيف وهي الخلية الأولى في المصفوفة. |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue) { get; } | للتحقق مما إذا كانت قيمة هذه الخلية خطأ. |
| [IsFormula](../../aspose.cells/cell/isformula) { get; } | يمثل إذا كانت الخلية المحددة تحتوي على صيغة. |
| [IsMerged](../../aspose.cells/cell/ismerged) { get; } | للتحقق مما إذا كانت الخلية جزءًا من نطاق مدمج أم لا. |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue) { get; } | يشير إلى ما إذا كانت القيمة الداخلية لهذه الخلية رقمية (عدد صحيح ومزدوج وتاريخ ووقت) |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula) { get; } | يشير إلى ما إذا كانت صيغة الخلية جزء من صيغة مشتركة. |
| [IsStyleSet](../../aspose.cells/cell/isstyleset) { get; } | يشير إلى ما إذا تم تعيين نمط الخلية. إذا تم إرجاع خطأ ، فهذا يعني أن هذه الخلية لها تنسيق افتراضي للخلية. |
| [IsTableFormula](../../aspose.cells/cell/istableformula) { get; } | يشير إلى ما إذا كانت هذه الخلية جزء من صيغة الجدول. |
| [Name](../../aspose.cells/cell/name) { get; } | يحصل على اسم الخلية. |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype) { get; } | يمثل نوع فئة تنسيق رقم هذه الخلية. |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula) { get; set; } | الحصول على أو تعيين صيغة R1C1 لملف[`Cell`](../cell) . |
| [Row](../../aspose.cells/cell/row) { get; } | الحصول على رقم الصف (على أساس الصفر) للخلية . |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex) { get; } | الحصول على فهرس النمط المشترك للخلية في تجمع الأنماط. |
| [StringValue](../../aspose.cells/cell/stringvalue) { get; } | الحصول على قيمة السلسلة الموجودة في الخلية. إذا كان نوع هذه الخلية عبارة عن سلسلة ، فقم بإرجاع قيمة السلسلة نفسها . بالنسبة لأنواع الخلايا الأخرى ، سيتم إرجاع قيمة السلسلة المنسقة (المنسقة بالنمط المحدد لهذه الخلية). يمكن الحصول عليها من Excel عند نسخ خلية كنص (مثل نسخ الخلية إلى محرر نصوص أو التصدير إلى ملف csv) . |
| [Type](../../aspose.cells/cell/type) { get; } | يمثل نوع قيمة الخلية. |
| [Value](../../aspose.cells/cell/value) { get; set; } | الحصول على القيمة الموجودة في هذه الخلية . |
| [Worksheet](../../aspose.cells/cell/worksheet) { get; } | الحصول على ورقة العمل الأصل . |

## طُرق

| اسم | وصف |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate#calculate)(CalculationOptions) | حساب صيغة الخلية . |
| [Characters](../../aspose.cells/cell/characters)(int, int) | إرجاع كائن أحرف يمثل نطاقًا من الأحرف داخل نص الخلية. |
| [Copy](../../aspose.cells/cell/copy)(Cell) | نسخ البيانات من خلية مصدر . |
| [Equals](../../aspose.cells/cell/equals#equals)(Cell) | للتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع كائن خلية آخر. |
| override [Equals](../../aspose.cells/cell/equals#equals_1)(object) | للتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية بأخرى. |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange)() | الحصول على نطاق الصفيف إذا كانت صيغة الخلية عبارة عن صيغة صفيف. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters)() | إرجاع كافة كائنات الأحرف التي تمثل نطاقًا من الأحرف داخل نص الخلية. |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters_1)(bool) | إرجاع كافة كائنات الأحرف التي تمثل نطاقًا من الأحرف داخل نص الخلية. |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult)() | الحصول على نتيجة التنسيق الشرطي . |
| [GetDependents](../../aspose.cells/cell/getdependents)(bool) | احصل على جميع الخلايا التي تشير صيغتها إلى هذه الخلية مباشرةً. |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation)(bool) | يحصل على كافة الخلايا التي تعتمد نتيجتها المحسوبة على هذه الخلية. |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle)() | الحصول على نمط عرض الخلية. إذا تأثرت هذه الخلية أيضًا بإعدادات أخرى مثل التنسيق الشرطي وكائنات القائمة وما إلى ذلك ، فقد يختلف نمط العرض عن الخلية. GetStyle () . |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle_1)(bool) | الحصول على نمط عرض الخلية. إذا كانت الخلية منسقة شرطيًا ، فلن يكون نمط العرض مطابقًا للخلية. GetStyle () . |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions)() | يحصل على شروط التنسيق التي تنطبق على هذه الخلية. |
| [GetFormula](../../aspose.cells/cell/getformula)(bool, bool) | احصل على صيغة هذه الخلية . |
| override [GetHashCode](../../aspose.cells/cell/gethashcode)() | يعمل كدالة تجزئة لنوع معين. |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue)() | الحصول على ارتفاع القيمة بوحدة البكسل . |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring)(bool) | الحصول على سلسلة html التي تحتوي على بيانات وبعض التنسيقات في هذه الخلية. |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange)() | إرجاع أ[`Range`](../range) كائن يمثل نطاقًا مدمجًا . |
| [GetPrecedents](../../aspose.cells/cell/getprecedents)() | الحصول على كافة المراجع التي تظهر في صيغة هذه الخلية. |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation)() | الحصول على كافة السابقات (مرجع للخلايا في المصنف الحالي) المستخدمة بواسطة صيغة هذه الخلية أثناء حسابها. |
| [GetStringValue](../../aspose.cells/cell/getstringvalue)(CellValueFormatStrategy) | الحصول على قيمة السلسلة من خلال استراتيجية منسقة محددة. |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle)() | الحصول على نمط الخلية . |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle_1)(bool) | إذا كانت checkBorders صحيحة ، فتحقق مما إذا كانت حدود الخلايا الأخرى ستؤثر على نمط هذه الخلية. |
| [GetTable](../../aspose.cells/cell/gettable)() | الحصول على الجدول الذي يحتوي على هذه الخلية. |
| [GetValidation](../../aspose.cells/cell/getvalidation)() | الحصول على التحقق المطبق على هذه الخلية. |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue)() | الحصول على قيمة التحقق التي تم تطبيقها على هذه الخلية. |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue)() | الحصول على عرض القيمة بوحدة البكسل . |
| [IsRichText](../../aspose.cells/cell/isrichtext)() | يشير إلى ما إذا كانت قيمة سلسلة الخلية نص منسق. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue)(bool) | يضع قيمة منطقية في الخلية. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_3)(DateTime) | يضع قيمة DateTime في الخلية. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_1)(double) | يضع قيمة مزدوجة في الخلية . |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_2)(int) | يضع قيمة عدد صحيح في الخلية . |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_4)(object) | يضع قيمة كائن في الخلية . |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_5)(string) | يضع قيمة سلسلة في الخلية . |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_6)(string, bool) | يضع قيمة سلسلة في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان ذلك مناسبًا. |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_7)(string, bool, bool) | يضع قيمة في الخلية ، إذا كان ذلك مناسبًا ، سيتم تحويل القيمة إلى نوع بيانات آخر وستتم إعادة تعيين تنسيق رقم الخلية. |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula)(bool) | إزالة صيغة الصفيف . |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula)(string, int, int) | يعين صيغة صفيف (صيغة صفيف قديمة تم إدخالها عبر CTRL + SHIFT + ENTER في ms excel) إلى نطاق من الخلايا . |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_1)(string, int, int, FormulaParseOptions) | تعيين صيغة صفيف إلى نطاق من الخلايا . |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | تعيين صيغة صفيف إلى نطاق من الخلايا . |
| [SetCharacters](../../aspose.cells/cell/setcharacters)(FontSetting[]) | تعيين تنسيق النص المنسق للخلية. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula)(string, FormulaParseOptions, bool) | لتعيين صيغة الصفيف الديناميكي وجعل الصيغة تنتشر في الخلايا المجاورة إن أمكن. |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | لتعيين صيغة الصفيف الديناميكي وجعل الصيغة تنتشر في الخلايا المجاورة إن أمكن. |
| [SetFormula](../../aspose.cells/cell/setformula#setformula_2)(string, object) | اضبط الصيغة وقيمة الصيغة . |
| [SetFormula](../../aspose.cells/cell/setformula#setformula)(string, FormulaParseOptions, object) | اضبط الصيغة وقيمة الصيغة . |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula)(string, int, int) | يعين صيغة لنطاق من الخلايا . |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_1)(string, int, int, FormulaParseOptions) | يعين صيغة لنطاق من الخلايا . |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | يعين صيغة لنطاق من الخلايا . |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle)(Style) | يضبط نمط الخلية. |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_2)(Style, bool) | تطبيق نمط الخلية . |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_1)(Style, StyleFlag) | تطبيق نمط الخلية . |
| override [ToString](../../aspose.cells/cell/tostring)() | إرجاع سلسلة تمثل كائن الخلية الحالي. |

### أمثلة

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

// ضع سلسلة في خلية
Cell cell = cells[0, 0];
cell.PutValue("Hello");

string first = cell.StringValue;
	
// ضع عددًا صحيحًا في خلية
cell = cells["B1"];
cell.PutValue(12);

int second = cell.IntValue;

// ضع مزدوج في خلية
cell = cells[0, 2];
cell.PutValue(-1.234);

double third = cell.DoubleValue;

// ضع صيغة في خلية
cell = cells["D1"];
cell.Formula = "=B1 + C1";

// ضع صيغة مجمعة: "sum (average (b1، c1)، b1)" في الخلية في b2
cell = cells["b2"];
cell.Formula = "=sum(average(b1,c1), b1)";

// تعيين نمط الخلية
Style style = cell.GetStyle();
// تعيين لون الخلفية
style.BackgroundColor = Color.Yellow;
// تعيين تنسيق الخلية
style.Font.Name = "Courier New";
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);



[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = exce.Worksheets(0).Cells

'ضع سلسلة في خلية
Dim cell as Cell = cells(0, 0)
cell.PutValue("Hello")

Dim first as String = cell.StringValue
	
// ضع عددًا صحيحًا في خلية
cell = cells("B1")
cell.PutValue(12)

Dim second as Integer = cell.IntValue

// ضع مزدوج في خلية
cell = cells(0, 2)
cell.PutValue(-1.234)

Dim third as Double = cell.DoubleValue

// ضع صيغة في خلية
cell = cells("D1")
cell.Formula = "=B1 + C1"

// ضع صيغة مجمعة: "sum (average (b1، c1)، b1)" في الخلية في b2
cell = cells("b2")
cell.Formula = "=sum(average(b1,c1), b1)"
	
// تعيين نمط الخلية
Dim style as Style = cell.GetStyle()

// تعيين لون الخلفية
style.BackgroundColor = Color.Yellow
// تعيين خط الخلية
style.Font.Name = "Courier New"
style.VerticalAlignment = TextAlignmentType.Top
cell.SetStyle(style)
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
