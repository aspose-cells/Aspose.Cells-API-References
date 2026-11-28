---
title: "Validation.InCellDropDown"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama özelliği. Veri doğrulamanın kabul edilebilir değerleri içeren bir açılır liste gösterip göstermediğini belirtir"
type: docs
url: /tr/net/aspose.cells/validation/incelldropdown/
---
## Validation.InCellDropDown property

Veri doğrulamasının kabul edilebilir değerleri içeren bir açılır liste gösterip göstermediğini belirtir.

```csharp
public bool InCellDropDown { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyInCellDropDownDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresi için bir doğrulama oluştur
            Validation validation = worksheet.Cells["A1"].GetValidation();
            
            // Doğrulama tipini değerli liste olarak ayarla
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Hücre içi açılır menüyü etkinleştir
            validation.InCellDropDown = true;

            // B1 hücresi için açılır menüsü olmadan başka bir doğrulama oluştur
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Formula1 = "Choice1,Choice2,Choice3";
            validation2.InCellDropDown = false;

            // Çalışma kitabını kaydedin
            workbook.Save("InCellDropDownDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


