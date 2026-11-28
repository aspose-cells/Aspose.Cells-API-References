---
title: "Validation.Operator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Validation özelliği. Veri doğrulama için operatörü temsil eder"
type: docs
url: /tr/net/aspose.cells/validation/operator/
---
## Validation.Operator property

Veri doğrulama için operatörü temsil eder.

```csharp
public OperatorType Operator { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyOperatorDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğrulama için örnek veri ekle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Bir doğrulama aralığı oluştur
            CellArea area = CellArea.CreateCellArea("B1", "B5");
            int validationIndex = worksheet.Validations.Add(area);
            Validation validation = worksheet.Validations[validationIndex];

            // Operator gösterimiyle doğrulama özelliklerini ayarla
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "30";
            validation.ShowError = true;
            validation.ErrorMessage = "Value must be between 10 and 30";

            // Çalışma kitabını kaydedin
            workbook.Save("ValidationOperatorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [OperatorType](../../operatortype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


