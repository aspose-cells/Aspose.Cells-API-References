---
title: "Enum ValidationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ValidationType enum. Veri doğrulama türünü temsil eder."
type: docs
url: /tr/net/aspose.cells/validationtype/
---
## ValidationType enumeration

Veri doğrulama türünü temsil eder.

```csharp
public enum ValidationType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| AnyValue | `0` | Herhangi bir değer doğrulama türü. |
| WholeNumber | `1` | Tam sayı doğrulama türü. |
| Decimal | `2` | Ondalık doğrulama türü. |
| List | `3` | Liste doğrulama türü. |
| Date | `4` | Tarih doğrulama türü. |
| Time | `5` | Saat doğrulama türü. |
| TextLength | `6` | Metin uzunluğu doğrulama türü. |
| Custom | `7` | Özel doğrulama türü. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationTypeDemo
    {
        public static void ValidationTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir doğrulama ekle
            ValidationCollection validations = worksheet.Validations;
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
            Validation validation = validations[validations.Add(area)];

            // Doğrulama türünü WholeNumber olarak ayarla
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";

            // Doğrulama için ek özellikler ayarlayın
            validation.InputMessage = "Please enter a whole number between 3 and 1234.";
            validation.InputTitle = "Whole Number Validation";
            validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
            validation.ErrorTitle = "Invalid Input";
            validation.ShowInput = true;
            validation.ShowError = true;

            // Çalışma kitabını kaydedin
            workbook.Save("ValidationTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


