---
title: "Validation.Copy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Validation yöntemi. Doğrulamayı kopyala"
type: docs
url: /tr/net/aspose.cells/validation/copy/
---
## Validation.Copy method

Doğrulamayı kopyala.

```csharp
public void Copy(Validation source, CopyOptions copyOption)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Doğrulama | Kaynak doğrulama. |
| copyOption | CopyOptions | Kopya seçeneği. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodCopyWithValidationCopyOptionsDemo
    {
        public static void Run()
        {
            // Örnek veri ve doğrulama içeren bir kaynak çalışma kitabı oluştur
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // Kaynak sayfaya örnek doğrulama ekle
            Validation sourceValidation = sourceSheet.Validations[sourceSheet.Validations.Add()];
            sourceValidation.Type = ValidationType.WholeNumber;
            sourceValidation.Operator = OperatorType.Between;
            sourceValidation.Formula1 = "10";
            sourceValidation.Formula2 = "20";
            
            // StartRow, StartColumn, EndRow, EndColumn ile CellArea oluştur
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            sourceValidation.AddArea(area);

            // Bir hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Hedef sayfaya bir doğrulama ekle (kopya ile üzerine yazılacak)
            Validation destValidation = destSheet.Validations[destSheet.Validations.Add()];
            destValidation.AddArea(area); // Reuse the same area definition

            // CopyOptions ile Copy yöntemini göster
            CopyOptions options = new CopyOptions();
            destValidation.Copy(sourceValidation, options);

            // Doğrulamanın doğru bir şekilde kopyalandığını doğrula
            Console.WriteLine("Validation Type: " + destValidation.Type);
            Console.WriteLine("Validation Formula1: " + destValidation.Formula1);
            Console.WriteLine("Validation Formula2: " + destValidation.Formula2);
        }
    }
}
```

### Ayrıca Bakınız

* class [CopyOptions](../../copyoptions/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


