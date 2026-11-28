---
title: "LoadOptions.CheckDataValid"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Şablon dosyasındaki verinin geçerli olup olmadığını kontrol edin"
type: docs
url: /tr/net/aspose.cells/loadoptions/checkdatavalid/
---
## LoadOptions.CheckDataValid property

Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol et.

```csharp
public bool CheckDataValid { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckDataValidDemo
    {
        public static void Run()
        {
            // CheckDataValid'i false olarak ayarlayarak yükleme seçenekleri oluşturun
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CheckDataValid = false;

            // Bu seçeneklerle çalışma kitabını yükleyin
            Workbook workbook = new Workbook("example.xlsx", options);

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstrasyon için bazı veri doğrulamaları ekleyin
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "10";
            validation.Formula2 = "100";

            // Doğrulama aralığını ayarla
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 10;
            area.EndColumn = 0;
            validation.AddArea(area);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


