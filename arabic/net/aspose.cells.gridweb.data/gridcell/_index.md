---
title: "الفئة GridCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.Data.GridCell. تمثل كائن خلية."
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

يمثل كائن خلية.

```csharp
public class GridCell
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue/) { get; } | يحصل على القيمة المنطقية الموجودة في الخلية. |
| [Column](../../aspose.cells.gridweb.data/gridcell/column/) { get; } | يحصل على رقم العمود (مبني على الصفر) للخلية. |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue/) { get; } | يحصل على قيمة DateTime الموجودة في الخلية. |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue/) { get; } | يحصل على القيمة النصية المنسقة لهذه الخلية. |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue/) { get; } | يحصل على القيمة المزدوجة الموجودة في الخلية. |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue/) { get; } | يحصل على القيمة العائمة الموجودة في الخلية. |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula/) { get; set; } | يحصل أو يعيّن صيغة لـ `GridCell`. |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring/) { get; set; } | يحصل ويضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية. |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue/) { get; } | يحصل على القيمة الصحيحة الموجودة في الخلية. |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset/) { get; } | يشير إلى ما إذا تم تعيين نمط الخلية. إذا تم إرجاع false، فهذا يعني أن هذه الخلية لديها تنسيق خلية افتراضي. |
| [Name](../../aspose.cells.gridweb.data/gridcell/name/) { get; } | يحصل على اسم الخلية. على سبيل المثال: A1, F102. |
| [Row](../../aspose.cells.gridweb.data/gridcell/row/) { get; } | يحصل على رقم الصف (مبني على الصفر) للخلية. |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue/) { get; } | يحصل على القيمة النصية الموجودة في الخلية. |
| [Style](../../aspose.cells.gridweb.data/gridcell/style/) { get; set; } | يحصل على نسخة من نمط الخلية. اضبط النمط للخلية. |
| [Type](../../aspose.cells.gridweb.data/gridcell/type/) { get; } | إرجاع نوع قيمة الخلية، يمكن الاطلاع على المعنى في GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value/) { get; set; } | يحصل على القيمة الموجودة في هذه الخلية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink/)() | يشير إلى ما إذا كانت هذه الخلية تحتوي على رابط خارجي. ينطبق فقط عندما تكون الخلية خلية صيغة. |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy/)(GridCell) | ينسخ البيانات من خلية المصدر. |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle/)(GridTableItemStyle) | انسخ النمط واضبط النمط للخلية |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment/)(string, string, bool) | ينشئ كائن تعليق لخلية. |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation/)(GridValidationType, bool) | ينشئ كائن تحقق لخلية. |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals/)(object) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع كائن خلية آخر. |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment/)() | احصل على كائن التعليق في هذه الخلية |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode/)() | يعمل كدالة تجزئة لنوع معين. |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue/)() | يحصل على عرض القيمة بوحدة البكسل. |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue/)() | يتحقق مما إذا كانت الصيغة يمكنها تقييم النتيجة بشكل صحيح. |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula/)() | يمثل ما إذا كانت الخلية المحددة تحتوي على صيغة. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue)(bool) | يضع قيمة منطقية في الخلية. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_3)(DateTime) | يضع قيمة تاريخ/وقت في الخلية. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_1)(double) | يضع قيمة مزدوجة في الخلية. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_2)(int) | يضع قيمة عددية صحيحة في الخلية. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_4)(object) | يضع قيمة كائن في الخلية. نفس طريقة setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_5)(string) | يضع قيمة نصية في الخلية. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_6)(string, bool) | يضع قيمة سلسلة في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان ذلك مناسبًا. |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | يضع قيمة في الخلية، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الأرقام للخلية. |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue/)(string) | يضبط قيمة الخلية بقيمة نصية ويضبط تنسيق الخلية بناءً على هذه القيمة. |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment/)() | يزيل كائن التعليق للخلية. |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation/)() | يزيل كائن التحقق للخلية. |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder/)(WebBorderStyle) | يضبط حدود (أعلى، أسفل، يسار ويمين) للخلية، جميع الحدود لها نفس نمط الحد. |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom/)(string) | يضبط التنسيق المخصص، null أو سلسلة فارغة يعني عدم وجود تنسيق مخصص. |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula/)(string, object) | عيّن الصيغة وقيمة الصيغة. |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype/)(int) | عيّن تنسيق العرض للأرقام والتواريخ |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring/#tostring)() | إرجاع سلسلة تمثل كائن Cell الحالي. |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality/) |  |

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


