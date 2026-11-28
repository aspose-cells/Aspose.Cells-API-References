---
title: "Cell.GetValidation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bu hücreye uygulanan doğrulamayı alır"
type: docs
url: /tr/net/aspose.cells/cell/getvalidation/
---
## Cell.GetValidation method

Bu hücreye uygulanan doğrulamayı al.

```csharp
public Validation GetValidation()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetValidationDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // B5 hücresine eriş ve doğrulama ekle
            Cell cell = worksheet.Cells["B5"];
            Validation validation = cell.GetValidation();
            
            // Doğrulama türünü ayarla ve mesajı göster
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "20";
            validation.ShowError = true;
            validation.ErrorMessage = "Enter value between 10 and 20";
            
            // Çalışma kitabını kaydedin
            workbook.Save("ValidationDemo.xlsx");
            
            // Doğrulamayı doğrula
            Validation retrievedValidation = cell.GetValidation();
            Console.WriteLine("Validation Type: " + retrievedValidation.Type);
            Console.WriteLine("Validation Message: " + retrievedValidation.ErrorMessage);
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


