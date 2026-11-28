---
title: "Worksheet.Validations"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasındaki veri doğrulama ayarları koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/worksheet/validations/
---
## Worksheet.Validations property

Çalışma sayfasındaki veri doğrulama ayarları koleksiyonunu alır.

```csharp
public ValidationCollection Validations { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyValidationsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine veri doğrulama ekle
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Option1,Option2,Option3";
            
            // Düzeltme: StartRow, StartColumn, EndRow, EndColumn ile CellArea oluştur
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // A1 hücresinden doğrulamayı al
            Validation cellValidation = worksheet.Validations.GetValidationInCell(0, 0);
            
            // Doğrulama tipini çıktı ver
            Console.WriteLine("Validation type in A1: " + cellValidation.Type);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ValidationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


