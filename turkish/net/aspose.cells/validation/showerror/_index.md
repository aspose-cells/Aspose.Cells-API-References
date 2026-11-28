---
title: "Validation.ShowError"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama özelliği. Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının gösterilip gösterilmeyeceğini belirtir"
type: docs
url: /tr/net/aspose.cells/validation/showerror/
---
## Validation.ShowError property

Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının gösterilip gösterilmeyeceğini belirtir.

```csharp
public bool ShowError { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyShowErrorDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresi için doğrulama oluştur
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            
            // Doğrulama özelliklerini ayarla
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            
            // Hata uyarısını yapılandırın
            validation.ShowError = true;
            validation.ErrorTitle = "Invalid Input";
            validation.ErrorMessage = "Value must be between 10 and 20";

            // Özellik kopyalamayı göstermek için başka bir doğrulama oluşturun
            Validation targetValidation = worksheet.Validations[worksheet.Validations.Add()];
            targetValidation.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 1, EndColumn = 0 });

            // İlk doğrulamadan ShowError ve ilgili özellikleri kopyalayın
            targetValidation.ShowError = validation.ShowError;
            targetValidation.ErrorTitle = validation.ErrorTitle;
            targetValidation.ErrorMessage = validation.ErrorMessage;

            // Çalışma kitabını kaydedin
            workbook.Save("ValidationShowErrorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


