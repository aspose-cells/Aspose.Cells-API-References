---
title: "Validation.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama özelliği. Veri doğrulama tipini temsil eder"
type: docs
url: /tr/net/aspose.cells/validation/type/
---
## Validation.Type property

Veri doğrulama tipini temsil eder.

```csharp
public ValidationType Type { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir doğrulama ekle
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.ErrorTitle = "Number Validation";
            validation.ErrorMessage = "Please enter a whole number";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });

            // Type özelliğini göster
            Console.WriteLine("Validation Type: " + validation.Type);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ValidationExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


