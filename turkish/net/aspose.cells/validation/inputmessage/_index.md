---
title: "Validation.InputMessage"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama özelliği. Veri doğrulama giriş mesajını temsil eder"
type: docs
url: /tr/net/aspose.cells/validation/inputmessage/
---
## Validation.InputMessage property

Veri doğrulama giriş mesajını temsil eder.

```csharp
public string InputMessage { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputMessageDemo
    {
        public static void Run()
        {
            // Çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğrulama oluştur
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.IgnoreBlank = true;
            validation.InCellDropDown = true;
            
            // Giriş mesajı özelliklerini ayarla
            validation.ShowInput = true;
            validation.InputTitle = "Selection Required";
            validation.InputMessage = "Please select either Yes or No from the dropdown";

            // Çalışma kitabını kaydedin
            workbook.Save("ValidationInputMessageDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


