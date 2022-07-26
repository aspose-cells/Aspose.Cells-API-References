---
title: GridCell
second_title: Aspose.Cells لمرجع .NET API
description: يمثل كائن خلية .
type: docs
weight: 150
url: /ar/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

يمثل كائن خلية .

```csharp
public class GridCell
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue) { get; } | الحصول على القيمة المنطقية الموجودة في الخلية. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column) { get; } | الحصول على رقم العمود (على أساس الصفر) للخلية . |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue) { get; } | الحصول على قيمة DateTime الموجودة في الخلية. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue) { get; } | الحصول على قيمة السلسلة المنسقة لهذه الخلية. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue) { get; } | الحصول على القيمة المزدوجة الموجودة في الخلية. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue) { get; } | الحصول على القيمة العائمة الموجودة في الخلية. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula) { get; set; } | الحصول على صيغة ملفCell . |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring) { get; set; } | الحصول على وتعيين سلسلة html التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue) { get; } | الحصول على قيمة العدد الصحيح الموجود في الخلية. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset) { get; } | يشير إلى ما إذا تم تعيين نمط الخلية. إذا تم إرجاع خطأ ، فهذا يعني أن هذه الخلية لها تنسيق افتراضي للخلية. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name) { get; } | الحصول على اسم الخلية. على سبيل المثال: A1 ، F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row) { get; } | الحصول على رقم الصف (على أساس الصفر) للخلية . |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue) { get; } | الحصول على قيمة السلسلة الموجودة في الخلية. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style) { get; set; } | الحصول على نسخة من نمط الخلية. قم بتعيين نمط الخلية. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type) { get; } | إرجاع نوع قيمة الخلية ، يمكن أن يرى المعنى GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value) { get; set; } | الحصول على القيمة الموجودة في هذه الخلية . |

## طُرق

| اسم | وصف |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink)() | يشير إلى ما إذا كانت هذه الخلية تحتوي على ارتباط خارجي . يتم تطبيقه فقط عندما تكون الخلية عبارة عن خلية صيغة. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy)(GridCell) | نسخ البيانات من خلية مصدر . |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle)(GridTableItemStyle) | انسخ النمط وقم بتعيين النمط للخلية |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment)(string, string, bool) | إنشاء كائن تعليق لخلية . |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation)(GridValidationType, bool) | إنشاء كائن تحقق لخلية . |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.gridweb.data/gridcell/getcellarea)() |  |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment)() | احصل على كائن تعليق على هذه الخلية |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode)() |  |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue)() | الحصول على عرض القيمة بوحدة البكسل . |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue)() | للتحقق مما إذا كانت الصيغة يمكنها تقييم النتيجة بشكل صحيح. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula)() | يمثل إذا كانت الخلية المحددة تحتوي على صيغة. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue)(bool) | يضع قيمة منطقية في الخلية. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_3)(DateTime) | يضع قيمة DateTime في الخلية. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_1)(double) | يضع قيمة مزدوجة في الخلية . |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_2)(int) | يضع قيمة int في الخلية. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_4)(object) | يضع قيمة كائن في الخلية. نفس setValue (كائن param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_5)(string) | يضع قيمة سلسلة في الخلية . |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_6)(string, bool) | يضع قيمة سلسلة في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان ذلك مناسبًا. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | يضع قيمة في الخلية ، إذا كان ذلك مناسبًا ، سيتم تحويل القيمة إلى نوع بيانات آخر وستتم إعادة تعيين تنسيق رقم الخلية. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue)(string) | يضبط قيمة الخلية بقيمة سلسلة وتعيين تنسيق الخلية بهذه القيمة. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment)() | يزيل كائن التعليق من الخلية . |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation)() | يزيل كائن التحقق من الخلية. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder)(WebBorderStyle) | تعيين الحدود (أعلى ، أسفل ، يسار ويمين) للخلية ، جميع الحدود لها نفس نمط الحدود. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom)(string) | يحدد التنسيق المخصص ، وتعني السلسلة الفارغة أو الفارغة عدم وجود تنسيق مخصص. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula)(string, object) | اضبط الصيغة وقيمة الصيغة . |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype)(int) | ضبط تنسيق عرض الأرقام والتواريخ |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring#tostring)() | إرجاع سلسلة تمثل كائن الخلية الحالي. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality) |  |

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* المجسم [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
