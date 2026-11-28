---
title: "Validation.InputTitle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Validation özelliği. Veri doğrulama giriş iletişim kutusunun başlığını temsil eder"
type: docs
url: /tr/net/aspose.cells/validation/inputtitle/
---
## Validation.InputTitle property

Veri doğrulama giriş iletişim kutusunun başlığını temsil eder.

```csharp
public string InputTitle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInputTitleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir doğrulama nesnesi oluştur
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.IgnoreBlank = true;
            
            // Doğrulama aralığını ayarla
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Doğrulama özelliklerini ayarla
            validation.Formula1 = "10";
            validation.Formula2 = "100";
            validation.Operator = OperatorType.Between;
            
            // Giriş mesajı özelliklerini ayarla
            validation.InputTitle = "Number Validation";
            validation.InputMessage = "Please enter a number between 10 and 100";
            
            // Çalışma kitabını kaydedin
            workbook.Save("ValidationInputTitleDemo.xlsx");
            
            // InputTitle özelliğini doğrula
            Console.WriteLine("Validation InputTitle: " + validation.InputTitle);
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


