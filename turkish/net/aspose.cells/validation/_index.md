---
title: Validation
second_title: Aspose.Cells for .NET API Referansı
description: Veri doğrulamasını temsil eder.settings.
type: docs
weight: 6200
url: /tr/net/aspose.cells/validation/
---
## Validation class

Veri doğrulamasını temsil eder.settings.

```csharp
public class Validation
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AlertStyle](../../aspose.cells/validation/alertstyle) { get; set; } | Doğrulama uyarı stilini temsil eder. |
| [Areas](../../aspose.cells/validation/areas) { get; } | Hepsini alır[`CellArea`](../cellarea) veri doğrulama ayarlarını içeren. |
| [ErrorMessage](../../aspose.cells/validation/errormessage) { get; set; } | Veri doğrulama hata mesajını temsil eder. |
| [ErrorTitle](../../aspose.cells/validation/errortitle) { get; set; } | Veri doğrulama hatası iletişim kutusunun başlığını temsil eder. |
| [Formula1](../../aspose.cells/validation/formula1) { get; set; } | Veri doğrulamayla ilişkili değeri veya ifadeyi temsil eder. |
| [Formula2](../../aspose.cells/validation/formula2) { get; set; } | Veri doğrulamayla ilişkili değeri veya ifadeyi temsil eder. |
| [IgnoreBlank](../../aspose.cells/validation/ignoreblank) { get; set; } | Aralık veri doğrulaması tarafından boş değerlere izin verilip verilmediğini gösterir. |
| [InCellDropDown](../../aspose.cells/validation/incelldropdown) { get; set; } | Veri doğrulamanın kabul edilebilir değerler içeren bir açılır liste gösterip göstermediğini gösterir. |
| [InputMessage](../../aspose.cells/validation/inputmessage) { get; set; } | Veri doğrulama giriş mesajını temsil eder. |
| [InputTitle](../../aspose.cells/validation/inputtitle) { get; set; } | Veri doğrulama girişi iletişim kutusunun başlığını temsil eder. |
| [Operator](../../aspose.cells/validation/operator) { get; set; } | Veri doğrulama operatörünü temsil eder. |
| [ShowError](../../aspose.cells/validation/showerror) { get; set; } | Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının görüntülenip görüntülenmeyeceğini belirtir. |
| [ShowInput](../../aspose.cells/validation/showinput) { get; set; } | Kullanıcı veri doğrulama aralığında bir hücre seçtiğinde veri doğrulama giriş mesajının görüntülenip görüntülenmeyeceğini belirtir. |
| [Type](../../aspose.cells/validation/type) { get; set; } | Veri doğrulama türünü temsil eder. |
| [Value1](../../aspose.cells/validation/value1) { get; set; } | Veri doğrulama ile ilişkili ilk değeri temsil eder. |
| [Value2](../../aspose.cells/validation/value2) { get; set; } | Veri doğrulamayla ilişkili ikinci değeri temsil eder. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AddArea](../../aspose.cells/validation/addarea#addarea)(CellArea) | Doğrulamayı alana uygular. |
| [AddArea](../../aspose.cells/validation/addarea#addarea_1)(CellArea, bool, bool) | Doğrulamayı alana uygular. |
| [AddAreas](../../aspose.cells/validation/addareas)(CellArea[], bool, bool) | Doğrulamayı verilen alanlara uygular. |
| [Copy](../../aspose.cells/validation/copy)(Validation, CopyOptions) | Doğrulamayı kopyala. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1)(bool, bool) | Bu doğrulamayla ilişkili değeri veya ifadeyi alır. |
| [GetFormula1](../../aspose.cells/validation/getformula1#getformula1_1)(bool, bool, int, int) | Belirli hücre için bu doğrulamayla ilişkili değeri veya ifadeyi alır. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2)(bool, bool) | Bu doğrulamayla ilişkili değeri veya ifadeyi alır. |
| [GetFormula2](../../aspose.cells/validation/getformula2#getformula2_1)(bool, bool, int, int) | Belirli hücre için bu doğrulamayla ilişkili değeri veya ifadeyi alır. |
| [GetListValue](../../aspose.cells/validation/getlistvalue)(int, int) | Belirtilen hücre için doğrulama listesi değerini alın. |
| [RemoveACell](../../aspose.cells/validation/removeacell)(int, int) | Hücredeki doğrulama ayarlarını kaldırın. |
| [RemoveArea](../../aspose.cells/validation/removearea)(CellArea) | Aralıktaki doğrulama ayarlarını kaldırın. |
| [RemoveAreas](../../aspose.cells/validation/removeareas)(CellArea[]) | Bu doğrulamayı verilen alanlardan kaldırır. |
| [SetFormula1](../../aspose.cells/validation/setformula1)(string, bool, bool) | Bu doğrulamayla ilişkili değeri veya ifadeyi ayarlar. |
| [SetFormula2](../../aspose.cells/validation/setformula2)(string, bool, bool) | Bu doğrulamayla ilişkili değeri veya ifadeyi ayarlar. |

### Örnekler

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

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
