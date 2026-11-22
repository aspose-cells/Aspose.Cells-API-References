---
title: "فئة Validation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.Validation."
type: docs
url: /ar/net/aspose.cells.gridweb/validation/
---
## Validation class

```csharp
[Obsolete("This class is obsolete; use  GridValidation instead")]
public class Validation : CellAttachObject
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Validation](validation/#constructor)() | البناء الافتراضي. |
| [Validation](validation/#constructor_1)(GridValidation) |  |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Cell](../../aspose.cells.gridweb.data/cellattachobject/cell/) { get; } | يحصل على الخلية النسبية للكائن. (موروث من [`CellAttachObject`](../../aspose.cells.gridweb.data/cellattachobject/).) |
| [ClientValidationFunction](../../aspose.cells.gridweb/validation/clientvalidationfunction/) { get; set; } | يحصل أو يعيّن اسم دالة جافاسكريبت للتحقق من صحة العميل. |
| [ClientValidationOpType](../../aspose.cells.gridweb/validation/clientvalidationoptype/) { get; set; } | يحصل أو يعيّن نوع عملية التحقق، Between/NotBetween/Equal/NotEqual/Greater/GreaterOrEqual/Less/LessOrEqual. |
| [ClientValidationValue1](../../aspose.cells.gridweb/validation/clientvalidationvalue1/) { get; set; } | يحصل أو يعيّن قيمة الهدف للمعامل 1 |
| [ClientValidationValue2](../../aspose.cells.gridweb/validation/clientvalidationvalue2/) { get; set; } | يحصل أو يعيّن قيمة الهدف للمعامل 2 |
| [IsRequired](../../aspose.cells.gridweb/validation/isrequired/) { get; set; } | يحصل أو يضبط ما إذا كانت قيمة الخلية مطلوبة. |
| [RegEx](../../aspose.cells.gridweb/validation/regex/) { get; set; } | يحصل أو يعيّن سلسلة التعبير النمطي. |
| [ValueArray](../../aspose.cells.gridweb/validation/valuearray/) { get; set; } |  |
| [ValueList](../../aspose.cells.gridweb/validation/valuelist/) { get; } | يحصل على كائن قائمة القيم. |
| [ValueText](../../aspose.cells.gridweb/validation/valuetext/) { get; set; } | مستخدم فقط في وقت التصميم. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [LoadValueList](../../aspose.cells.gridweb/validation/loadvaluelist/)(DataView, string, string, bool) | يقوم بتحميل قائمة القيم من كائن DataView. يمكنك تحديد حقل القيمة وحقل النص في DataView. سيتم دمج كل زوج من القيمة والنص في سلسلة واحدة، مع فاصلة بينها. |

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. يرجى استخدام GridValidation بدلاً منها. سيتم إزالة هذه الفئة بعد 6 أشهر من أغسطس 2014. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### انظر أيضًا

* class [CellAttachObject](../../aspose.cells.gridweb.data/cellattachobject/)
* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


