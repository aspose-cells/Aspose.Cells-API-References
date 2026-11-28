---
title: "Validation.Formula2"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama özelliği. Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder"
type: docs
url: /tr/net/aspose.cells/validation/formula2/
---
## Validation.Formula2 property

Veri doğrulama ile ilişkili değeri veya ifadeyi temsil eder.

```csharp
public string Formula2 { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyFormula2Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            sheet.Cells["B3"].PutValue(100);
            sheet.Cells["B7"].PutValue(50);
            
            // B7 hücresi için doğrulama oluştur
            Validation validation = sheet.Cells["B7"].GetValidation();
            
            // Doğrulama tipini ve formüllerini ayarla
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "=B3";  // Demonstrating Formula2 usage
            
            // Doğrulamayı uygula
            CellArea area = new CellArea();
            area.StartRow = 6;
            area.StartColumn = 1;
            area.EndRow = 6;
            area.EndColumn = 1;
            validation.AddArea(area);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ValidationFormula2Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


