---
title: GridCell
second_title: Aspose.Cells لمرجع .NET API
description: يمثل كائن خلية .
type: docs
weight: 370
url: /ar/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

يمثل كائن خلية .

```csharp
public class GridCell
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue) { get; } | الحصول على القيمة المنطقية الموجودة في الخلية. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column) { get; } | الحصول على رقم العمود (على أساس الصفر) للخلية . |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue) { get; } | الحصول على قيمة DateTime الموجودة في الخلية. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue) { get; } | الحصول على قيمة السلسلة المنسقة لهذه الخلية. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue) { get; } | الحصول على القيمة المزدوجة الموجودة في الخلية. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue) { get; } | الحصول على القيمة العائمة الموجودة في الخلية. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula) { get; set; } | الحصول على صيغة ملفCell . |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring) { get; set; } | الحصول على وتعيين سلسلة html التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue) { get; } | الحصول على قيمة العدد الصحيح الموجود في الخلية. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset) { get; } | يشير إلى ما إذا تم تعيين نمط الخلية. إذا تم إرجاع خطأ ، فهذا يعني أن هذه الخلية لها تنسيق افتراضي للخلية. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name) { get; } | الحصول على اسم الخلية. على سبيل المثال: A1 ، F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected) { get; set; } | يشير إلى ما إذا كانت الخلية محمية. إذا كانت القيمة "صحيحة" ، فلا يمكن للمستخدم تعديل الخلية من خلال واجهة المستخدم. هذه السمة ليس لها علاقة بالخاصية Style.CellLocked ولن يتم حفظها في الملف عند تم تصدير بيانات الشبكة . القيمة الافتراضية هي "خطأ" . |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row) { get; } | الحصول على رقم الصف (على أساس الصفر) للخلية . |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue) { get; } | الحصول على قيمة السلسلة الموجودة في الخلية. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style) { get; set; } | الحصول على نسخة من نمط الخلية. قم بتعيين نمط الخلية. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type) { get; } | إرجاع نوع قيمة الخلية ، يمكن أن يرى المعنى GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value) { get; set; } | الحصول على القيمة الموجودة في هذه الخلية . |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet) { get; } | الحصول على كائن ورقة العمل . |

## طُرق

| اسم | وصف |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink)() | يشير إلى ما إذا كانت هذه الخلية تحتوي على ارتباط خارجي . يتم تطبيقه فقط عندما تكون الخلية عبارة عن خلية صيغة. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy)(GridCell) | نسخ البيانات من خلية مصدر . |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle)(Style) | انسخ النمط وقم بتعيين النمط للخلية |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont)() | الحصول على خط الخلية. عند تغيير الخط ، يجب استدعاء طريقة "SetFont" ، لتعيين الخط على الخلية. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor)() | الحصول على لون خط الخلية. عند تغيير اللون ، يجب استدعاء طريقة "SetFontColor" ، لتعيين لون الخط على الخلية. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle)() | الحصول على نمط الخلية. عند تغيير النمط ، يجب عليك استدعاء طريقة "SetStyle" ، لتعيين النمط على الخلية. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation)() | يحصل على التحقق الذي تم تطبيقه على هذه الخلية. إذا لم يتم تعيينه ، فسيتم إرجاعه فارغًا. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue)() | الحصول على عرض القيمة بوحدة البكسل . |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet)() | الحصول على ورقة العمل الأصل . |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue)() | للتحقق مما إذا كانت الصيغة يمكنها تقييم النتيجة بشكل صحيح. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula)() | يمثل إذا كانت الخلية المحددة تحتوي على صيغة. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue)(bool) | يضع قيمة منطقية في الخلية. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_3)(DateTime) | يضع قيمة DateTime في الخلية. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_1)(double) | يضع قيمة مزدوجة في الخلية . |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_2)(int) | يضع قيمة int في الخلية. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_4)(object) | يضع قيمة كائن في الخلية. نفس setValue (كائن param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_5)(string) | يضع قيمة سلسلة في الخلية . |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_6)(string, bool) | يضع قيمة سلسلة في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان ذلك مناسبًا. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | يضع قيمة في الخلية ، إذا كان ذلك مناسبًا ، سيتم تحويل القيمة إلى نوع بيانات آخر وستتم إعادة تعيين تنسيق رقم الخلية. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue)(string) | يضبط قيمة الخلية بقيمة سلسلة وتعيين تنسيق الخلية بهذه القيمة. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue)(object) | إذا كانت القيمة عبارة عن صيغة ، فإن هذه الطريقة تحدد قيمة الخلية على أنها FormulaType ، |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom)(string) | يحدد التنسيق المخصص ، وتعني السلسلة الفارغة أو الفارغة عدم وجود تنسيق مخصص. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont)(Font) | تعيين الخط على الخلية . لتحسين الأداء ، قم بتنفيذ طريقة "SetFont" ، لا تنفذ خاصية "الخط" . |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor)(Color) | تعيين لون الخط إلى الخلية. لتحسين الأداء ، قم بتنفيذ طريقة "SetFontColor" ، لا تنفذ خاصية "لون الخط". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula)(string, object) | اضبط الصيغة وقيمة الصيغة . |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype)(int) | ضبط تنسيق عرض الأرقام والتواريخ |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle)(Style) | تعيين النمط على الخلية . لتحسين الأداء ، قم بتنفيذ طريقة "SetStyle" ، لا تنفذ خاصية "النمط" . |
| [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring#tostring)() | إرجاع سلسلة تمثل كائن الخلية الحالي. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality) |  |

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* المجسم [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
