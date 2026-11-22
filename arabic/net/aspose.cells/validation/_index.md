---
title: "فئة Validation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Validation. يمثل إعدادات التحقق من البيانات"
type: docs
url: /ar/net/aspose.cells/validation/
---
## Validation class

يمثل إعدادات التحقق من صحة البيانات.

```csharp
public class Validation
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle/) { get; set; } | يمثل نمط تنبيه التحقق. |
| [Areas](../../aspose.cells/validation/areas/) { get; } | يحصل على جميع [`CellArea`](../cellarea/) التي تحتوي على إعدادات التحقق من البيانات. |
| [ErrorMessage](../../aspose.cells/validation/errormessage/) { get; set; } | يمثل رسالة خطأ التحقق من البيانات. |
| [ErrorTitle](../../aspose.cells/validation/errortitle/) { get; set; } | يمثل عنوان مربع حوار خطأ التحقق من البيانات. |
| [Formula1](../../aspose.cells/validation/formula1/) { get; set; } | يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات. |
| [Formula2](../../aspose.cells/validation/formula2/) { get; set; } | يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank/) { get; set; } | يشير إلى ما إذا كانت القيم الفارغة مسموح بها في التحقق من البيانات للنطاق. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown/) { get; set; } | يشير إلى ما إذا كان التحقق من البيانات يعرض قائمة منسدلة تحتوي على القيم المقبولة. |
| [InputMessage](../../aspose.cells/validation/inputmessage/) { get; set; } | يمثل رسالة الإدخال للتحقق من البيانات. |
| [InputTitle](../../aspose.cells/validation/inputtitle/) { get; set; } | يمثل عنوان مربع حوار إدخال التحقق من البيانات. |
| [Operator](../../aspose.cells/validation/operator/) { get; set; } | يمثل العامل للتحقق من البيانات. |
| [ShowError](../../aspose.cells/validation/showerror/) { get; set; } | يشير إلى ما إذا كانت رسالة خطأ التحقق من البيانات ستُعرض كلما أدخل المستخدم بيانات غير صالحة. |
| [ShowInput](../../aspose.cells/validation/showinput/) { get; set; } | يشير إلى ما إذا كانت رسالة إدخال التحقق من البيانات ستُعرض كلما اختار المستخدم خلية في نطاق التحقق من البيانات. |
| [Type](../../aspose.cells/validation/type/) { get; set; } | يمثل نوع التحقق من البيانات. |
| [Value1](../../aspose.cells/validation/value1/) { get; set; } | يمثل القيمة الأولى المرتبطة بالتحقق من البيانات. |
| [Value2](../../aspose.cells/validation/value2/) { get; set; } | يمثل القيمة الثانية المرتبطة بالتحقق من البيانات. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea/#addarea)(CellArea) | يطبق التحقق على المنطقة. |
| [AddArea](../../aspose.cells/validation/addarea/#addarea_1)(CellArea, bool, bool) | يطبق التحقق على المنطقة. |
| [AddAreas](../../aspose.cells/validation/addareas/)(CellArea[], bool, bool) | يطبق التحقق على المناطق المحددة. |
| [Copy](../../aspose.cells/validation/copy/)(Validation, CopyOptions) | نسخ التحقق. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1)(bool, bool) | يحصل على القيمة أو التعبير المرتبط بهذا التحقق. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1_1)(bool, bool, int, int) | يحصل على القيمة أو التعبير المرتبط بهذا التحقق للخلية المحددة. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2)(bool, bool) | يحصل على القيمة أو التعبير المرتبط بهذا التحقق. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2_1)(bool, bool, int, int) | يحصل على القيمة أو التعبير المرتبط بهذا التحقق للخلية المحددة. |
| [GetListValue](../../aspose.cells/validation/getlistvalue/)(int, int) | احصل على القيمة لقائمة التحقق للخلية المحددة. |
| [GetValue](../../aspose.cells/validation/getvalue/)(int, int, bool) | احصل على قيمة التحقق على الخلية المحددة. |
| [RemoveACell](../../aspose.cells/validation/removeacell/)(int, int) | إزالة إعدادات التحقق في الخلية. |
| [RemoveArea](../../aspose.cells/validation/removearea/)(CellArea) | إزالة إعدادات التحقق في النطاق. |
| [RemoveAreas](../../aspose.cells/validation/removeareas/)(CellArea[]) | يزيل هذا التحقق من المناطق المحددة. |
| [SetFormula1](../../aspose.cells/validation/setformula1/)(string, bool, bool) | يضبط القيمة أو التعبير المرتبط بهذا التحقق. |
| [SetFormula2](../../aspose.cells/validation/setformula2/)(string, bool, bool) | يضبط القيمة أو التعبير المرتبط بهذا التحقق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationDemo
    {
        public static void ValidationExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعريف منطقة خلايا للتحقق
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // الوصول إلى مجموعة التحققات
            ValidationCollection validations = worksheet.Validations;

            // إضافة تحقق جديد إلى المجموعة
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // تعيين خصائص التحقق
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;

            // احفظ المصنف
            workbook.Save("ValidationExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


