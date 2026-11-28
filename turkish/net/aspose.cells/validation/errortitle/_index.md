---
title: "Validation.ErrorTitle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama özelliği. Veri doğrulama hata iletişim kutusunun başlığını temsil eder"
type: docs
url: /tr/net/aspose.cells/validation/errortitle/
---
## Validation.ErrorTitle property

Veri doğrulama hata iletişim kutusunun başlığını temsil eder.

```csharp
public string ErrorTitle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyErrorTitleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(0, 0, 1, 1))];
            
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "3";
            validation.Formula2 = "1234";
            
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 3 and 1234";
            validation.ShowError = true;

            workbook.Save("ValidationErrorTitleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


