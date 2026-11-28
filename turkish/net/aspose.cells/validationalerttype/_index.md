---
title: "Enum ValidationAlertType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ValidationAlertType enum. Veri doğrulama uyarı stilini temsil eder"
type: docs
url: /tr/net/aspose.cells/validationalerttype/
---
## ValidationAlertType enumeration

Veri doğrulama uyarı stilini temsil eder.

```csharp
public enum ValidationAlertType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Information | `0` | Bilgi uyarı stili. |
| Stop | `1` | Durdurma uyarı stili. |
| Warning | `2` | Uyarı uyarı stili. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationAlertTypeDemo
    {
        public static void ValidationAlertTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğrulama için bir hücre alanı tanımlayın
            CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);

            // Çalışma sayfasına bir doğrulama ekle
            ValidationCollection validations = worksheet.Validations;
            int validationIndex = validations.Add(area);
            Validation validation = validations[validationIndex];

            // Doğrulama özelliklerini ayarla
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            validation.AlertStyle = ValidationAlertType.Stop; // Using the ValidationAlertType enum
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Please enter a number between 3 and 1234.";
            validation.ShowError = true;

            // Çalışma kitabını kaydedin
            workbook.Save("ValidationAlertTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


