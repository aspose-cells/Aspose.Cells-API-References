---
title: "Sınıf Validation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Validation sınıfı. Veri doğrulama ayarlarını temsil eder"
type: docs
url: /tr/net/aspose.cells/validation/
---
## Validation class

Veri doğrulama ayarlarını temsil eder.

```csharp
public class Validation
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle/) { get; set; } | Doğrulama uyarı stilini temsil eder. |
| [Areas](../../aspose.cells/validation/areas/) { get; } | Veri doğrulama ayarlarını içeren tüm [`CellArea`](../cellarea/) öğelerini alır. |
| [ErrorMessage](../../aspose.cells/validation/errormessage/) { get; set; } | Veri doğrulama hata mesajını temsil eder. |
| [ErrorTitle](../../aspose.cells/validation/errortitle/) { get; set; } | Veri doğrulama hata iletişim kutusunun başlığını temsil eder. |
| [Formula1](../../aspose.cells/validation/formula1/) { get; set; } | Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder. |
| [Formula2](../../aspose.cells/validation/formula2/) { get; set; } | Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank/) { get; set; } | Aralık veri doğrulamasının boş değerleri izin verip vermediğini gösterir. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown/) { get; set; } | Veri doğrulamasının kabul edilebilir değerleri içeren bir açılır liste gösterip göstermediğini belirtir. |
| [InputMessage](../../aspose.cells/validation/inputmessage/) { get; set; } | Veri doğrulama giriş mesajını temsil eder. |
| [InputTitle](../../aspose.cells/validation/inputtitle/) { get; set; } | Veri doğrulama giriş iletişim kutusunun başlığını temsil eder. |
| [Operator](../../aspose.cells/validation/operator/) { get; set; } | Veri doğrulama için operatörü temsil eder. |
| [ShowError](../../aspose.cells/validation/showerror/) { get; set; } | Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının gösterilip gösterilmeyeceğini belirtir. |
| [ShowInput](../../aspose.cells/validation/showinput/) { get; set; } | Kullanıcı veri doğrulama aralığındaki bir hücreyi seçtiğinde veri doğrulama giriş mesajının gösterilip gösterilmeyeceğini belirtir. |
| [Type](../../aspose.cells/validation/type/) { get; set; } | Veri doğrulama tipini temsil eder. |
| [Value1](../../aspose.cells/validation/value1/) { get; set; } | Veri doğrulama ile ilişkili ilk değeri temsil eder. |
| [Value2](../../aspose.cells/validation/value2/) { get; set; } | Veri doğrulama ile ilişkili ikinci değeri temsil eder. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea/#addarea)(CellArea) | Doğrulamayı alana uygular. |
| [AddArea](../../aspose.cells/validation/addarea/#addarea_1)(CellArea, bool, bool) | Doğrulamayı alana uygular. |
| [AddAreas](../../aspose.cells/validation/addareas/)(CellArea[], bool, bool) | Doğrulamayı verilen alanlara uygular. |
| [Copy](../../aspose.cells/validation/copy/)(Validation, CopyOptions) | Doğrulamayı kopyala. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1)(bool, bool) | Bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [GetFormula1](../../aspose.cells/validation/getformula1/#getformula1_1)(bool, bool, int, int) | Belirli hücre için bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2)(bool, bool) | Bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [GetFormula2](../../aspose.cells/validation/getformula2/#getformula2_1)(bool, bool, int, int) | Belirli hücre için bu doğrulama ile ilişkili değeri veya ifadeyi alır. |
| [GetListValue](../../aspose.cells/validation/getlistvalue/)(int, int) | Belirtilen hücre için doğrulama listesinin değerini al. |
| [GetValue](../../aspose.cells/validation/getvalue/)(int, int, bool) | Belirli hücredeki doğrulamanın değerini al. |
| [RemoveACell](../../aspose.cells/validation/removeacell/)(int, int) | Hücredeki doğrulama ayarlarını kaldır. |
| [RemoveArea](../../aspose.cells/validation/removearea/)(CellArea) | Aralıktaki doğrulama ayarlarını kaldır. |
| [RemoveAreas](../../aspose.cells/validation/removeareas/)(CellArea[]) | Bu doğrulamayı verilen alanlardan kaldırır. |
| [SetFormula1](../../aspose.cells/validation/setformula1/)(string, bool, bool) | Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar. |
| [SetFormula2](../../aspose.cells/validation/setformula2/)(string, bool, bool) | Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationDemo
    {
        public static void ValidationExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğrulama için bir hücre alanı tanımla
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Doğrulama koleksiyonuna eriş
            ValidationCollection validations = worksheet.Validations;

            // Koleksiyona yeni bir doğrulama ekle
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Doğrulama özelliklerini ayarla
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

            // Çalışma kitabını kaydedin
            workbook.Save("ValidationExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


