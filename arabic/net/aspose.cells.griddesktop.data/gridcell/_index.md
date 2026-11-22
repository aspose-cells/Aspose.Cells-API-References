---
title: "الفئة GridCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridDesktop.Data.GridCell. تمثل كائن خلية"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

يمثل كائن خلية.

```csharp
public class GridCell
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue/) { get; } | يحصل على القيمة المنطقية الموجودة في الخلية. |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column/) { get; } | يحصل على رقم العمود (مبني على الصفر) للخلية. |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue/) { get; } | يحصل على قيمة DateTime الموجودة في الخلية. |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue/) { get; } | يحصل على القيمة النصية المنسقة لهذه الخلية. |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue/) { get; } | يحصل على القيمة المزدوجة الموجودة في الخلية. |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue/) { get; } | يحصل على القيمة العائمة الموجودة في الخلية. |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula/) { get; set; } | يحصل أو يضبط صيغة الخلية. |
| [HasCustomStyle](../../aspose.cells.griddesktop.data/gridcell/hascustomstyle/) { get; } | يشير إلى ما إذا كانت هذه الخلية لديها إعدادات نمط مخصصة (مختلفة عن الإعداد الافتراضي الموروث من الصف أو العمود أو دفتر العمل المقابل). |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring/) { get; set; } | يحصل ويضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية. |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue/) { get; } | يحصل على القيمة الصحيحة الموجودة في الخلية. |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset/) { get; } | يشير إلى ما إذا تم تعيين نمط الخلية. إذا تم إرجاع false، فهذا يعني أن هذه الخلية لديها تنسيق خلية افتراضي. |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location/) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name/) { get; } | يحصل على اسم الخلية. على سبيل المثال: A1, F102. |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected/) { get; set; } | يشير إلى ما إذا كانت الخلية محمية. إذا كانت القيمة "true"، لا يمكن للمستخدم تعديل الخلية عبر واجهة المستخدم. هذه الخاصية لا علاقة لها بخصية Style.CellLocked ولن يتم حفظها في الملف عند تصدير بيانات الشبكة. القيمة الافتراضية هي "false". |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row/) { get; } | يحصل على رقم الصف (مبني على الصفر) للخلية. |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue/) { get; } | يحصل على القيمة النصية الموجودة في الخلية. |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style/) { get; set; } | يحصل على نسخة من نمط الخلية. اضبط النمط للخلية. |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type/) { get; } | إرجاع نوع قيمة الخلية، يمكن الاطلاع على المعنى في GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value/) { get; set; } | يحصل على القيمة الموجودة في هذه الخلية. |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet/) { get; } | يحصل على كائن ورقة العمل. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink/)() | يشير إلى ما إذا كانت هذه الخلية تحتوي على رابط خارجي. ينطبق فقط عندما تكون الخلية خلية صيغة. |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy/)(GridCell) | ينسخ البيانات من خلية المصدر. |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle/)(Style) | انسخ النمط واضبط النمط للخلية |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals/)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea/)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont/)() | يحصل على خط الخلية. عند تغيير الخط، يجب استدعاء طريقة "SetFont" لتعيين الخط للخلية. |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor/)() | يحصل على لون خط الخلية. عند تغيير اللون، يجب استدعاء طريقة "SetFontColor" لتعيين لون الخط للخلية. |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode/)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle/)() | يحصل على نمط الخلية. عند تغيير النمط، يجب استدعاء طريقة "SetStyle" لتعيين النمط للخلية. |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation/)() | يحصل على التحقق الذي تم تطبيقه على هذه الخلية. إذا لم يتم تعيينه، إرجاع null. |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue/)() | يحصل على عرض القيمة بوحدة البكسل. |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet/)() | يحصل على ورقة العمل الأم. |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue/)() | يتحقق مما إذا كانت الصيغة يمكنها تقييم النتيجة بشكل صحيح. |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula/)() | يمثل ما إذا كانت الخلية المحددة تحتوي على صيغة. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue)(bool) | يضع قيمة منطقية في الخلية. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_3)(DateTime) | يضع قيمة تاريخ/وقت في الخلية. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_1)(double) | يضع قيمة مزدوجة في الخلية. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_2)(int) | يضع قيمة عددية صحيحة في الخلية. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_4)(object) | يضع قيمة كائن في الخلية. نفس طريقة setValue(Object param_object) |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_5)(string) | يضع قيمة نصية في الخلية. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_6)(string, bool) | يضع قيمة سلسلة في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان ذلك مناسبًا. |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue/#putvalue_7)(string, bool, bool) | يضع قيمة في الخلية، إذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة ضبط تنسيق الأرقام للخلية. |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue/)(string) | يضبط قيمة الخلية بقيمة نصية ويضبط تنسيق الخلية بناءً على هذه القيمة. |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue/)(object) | إذا كانت القيمة صيغة، هذه الطريقة تضبط قيمة الخلية كـ FormulaType، |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom/)(string) | يضبط التنسيق المخصص، null أو سلسلة فارغة يعني عدم وجود تنسيق مخصص. |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont/)(Font) | يضبط الخط للخلية. لتحسين الأداء، نفّذ طريقة "SetFont"، لا تنفّذ خاصية "Font". |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor/)(Color) | يضبط لون الخط للخلية. لتحسين الأداء، نفّذ طريقة "SetFontColor"، لا تنفّذ خاصية "FontColor". |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula/)(string, object) | عيّن الصيغة وقيمة الصيغة. |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype/)(int) | عيّن تنسيق العرض للأرقام والتواريخ |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle/)(Style) | يضبط النمط للخلية. لتحسين الأداء، نفّذ طريقة "SetStyle"، لا تنفّذ خاصية "Style". |
| override [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring/)() | إرجاع سلسلة تمثل كائن Cell الحالي. |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality/) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality/) |  |

### انظر أيضًا

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


