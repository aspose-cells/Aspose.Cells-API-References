---
title: Validation
second_title: Aspose.Cells لمرجع .NET API
description: يمثل إعدادات التحقق من صحة البيانات.
type: docs
weight: 6200
url: /ar/net/aspose.cells/validation/
---
## Validation class

يمثل إعدادات التحقق من صحة البيانات.

```csharp
public class Validation
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle) { get; set; } | يمثل نمط تنبيه التحقق. |
| [Areas](../../aspose.cells/validation/areas) { get; } | يحصل على الكل[`CellArea`](../cellarea) التي تحتوي على إعدادات التحقق من صحة البيانات. |
| [ErrorMessage](../../aspose.cells/validation/errormessage) { get; set; } | يمثل رسالة خطأ التحقق من صحة البيانات. |
| [ErrorTitle](../../aspose.cells/validation/errortitle) { get; set; } | يمثل عنوان مربع حوار خطأ التحقق من صحة البيانات. |
| [Formula1](../../aspose.cells/validation/formula1) { get; set; } | يمثل القيمة أو التعبير المرتبط بالتحقق من صحة البيانات. |
| [Formula2](../../aspose.cells/validation/formula2) { get; set; } | يمثل القيمة أو التعبير المرتبط بالتحقق من صحة البيانات. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank) { get; set; } | يشير إلى ما إذا كانت القيم الفارغة مسموحًا بها من خلال التحقق من صحة بيانات النطاق. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown) { get; set; } | يشير إلى ما إذا كان التحقق من صحة البيانات يعرض قائمة منسدلة تحتوي على قيم مقبولة. |
| [InputMessage](../../aspose.cells/validation/inputmessage) { get; set; } | يمثل رسالة إدخال التحقق من صحة البيانات. |
| [InputTitle](../../aspose.cells/validation/inputtitle) { get; set; } | يمثل عنوان مربع حوار إدخال التحقق من صحة البيانات. |
| [Operator](../../aspose.cells/validation/operator) { get; set; } | يمثل المشغل للتحقق من صحة البيانات. |
| [ShowError](../../aspose.cells/validation/showerror) { get; set; } | يشير إلى ما إذا كان سيتم عرض رسالة خطأ التحقق من صحة البيانات عندما يقوم المستخدم بإدخال بيانات غير صالحة. |
| [ShowInput](../../aspose.cells/validation/showinput) { get; set; } | يشير إلى ما إذا كان سيتم عرض رسالة إدخال التحقق من صحة البيانات عندما يحدد المستخدم خلية في نطاق التحقق من صحة البيانات. |
| [Type](../../aspose.cells/validation/type) { get; set; } | يمثل نوع التحقق من صحة البيانات. |
| [Value1](../../aspose.cells/validation/value1) { get; set; } | يمثل القيمة الأولى المرتبطة بالتحقق من صحة البيانات. |
| [Value2](../../aspose.cells/validation/value2) { get; set; } | يمثل القيمة الثانية المرتبطة بالتحقق من صحة البيانات. |

## طُرق

| اسم | وصف |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea#addarea)(CellArea) | يتم تطبيق التحقق على المنطقة . |
| [AddArea](../../aspose.cells/validation/addarea#addarea_1)(CellArea, bool, bool) | يتم تطبيق التحقق على المنطقة . |
| [AddAreas](../../aspose.cells/validation/addareas)(CellArea[], bool, bool) | يطبق التحقق على مناطق معينة. |
| [Copy](../../aspose.cells/validation/copy)(Validation, CopyOptions) | نسخ التحقق. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1)(bool, bool) | الحصول على القيمة أو التعبير المرتبط بعملية التحقق هذه. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1_1)(bool, bool, int, int) | الحصول على القيمة أو التعبير المرتبط بعملية التحقق من الصحة لخلية معينة. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2)(bool, bool) | الحصول على القيمة أو التعبير المرتبط بعملية التحقق هذه. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2_1)(bool, bool, int, int) | الحصول على القيمة أو التعبير المرتبط بعملية التحقق من الصحة لخلية معينة. |
| [GetListValue](../../aspose.cells/validation/getlistvalue)(int, int) | احصل على القيمة لقائمة التحقق من صحة الخلية المحددة. |
| [RemoveACell](../../aspose.cells/validation/removeacell)(int, int) | قم بإزالة إعدادات التحقق من صحة الخلية . |
| [RemoveArea](../../aspose.cells/validation/removearea)(CellArea) | قم بإزالة إعدادات التحقق من الصحة في النطاق . |
| [RemoveAreas](../../aspose.cells/validation/removeareas)(CellArea[]) | يزيل هذا التحقق من الصحة من مناطق معينة . |
| [SetFormula1](../../aspose.cells/validation/setformula1)(string, bool, bool) | يعيّن القيمة أو التعبير المرتبط بعملية التحقق هذه. |
| [SetFormula2](../../aspose.cells/validation/setformula2)(string, bool, bool) | يعيّن القيمة أو التعبير المرتبط بعملية التحقق هذه. |

### أمثلة

```csharp
[C#]
Workbook workbook = new Workbook();
ValidationCollection validations = workbook.Worksheets[0].Validations;
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
Validation validation = validations[validations.Add(area)];
validation.Type = Aspose.Cells.ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "3";
validation.Formula2 = "1234";

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim validations as ValidationCollection  = workbook.Worksheets(0).Validations
Dim area as CellArea = CellArea.CreateCellArea(0, 0, 1, 1);
Dim validation as Validation = validations(validations.Add(area))
validation.Type = ValidationType.WholeNumber
validation.Operator = OperatorType.Between
validation.Formula1 = "3"
validation.Formula2 = "1234"
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
