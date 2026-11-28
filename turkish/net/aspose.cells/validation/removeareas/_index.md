---
title: "Validation.RemoveAreas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama yöntemi. Bu doğrulamayı verilen alanlardan kaldırır"
type: docs
url: /tr/net/aspose.cells/validation/removeareas/
---
## Validation.RemoveAreas method

Bu doğrulamayı verilen alanlardan kaldırır.

```csharp
public void RemoveAreas(CellArea[] areas)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| alanlar | CellArea[] | bu doğrulama ayarlarının kaldırılması gereken alanlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodRemoveAreasWithCellAreaArrayDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına veri doğrulaması ekle
            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            
            // Doğrulama ayarlarını yapılandır
            validation.Type = ValidationType.WholeNumber;
            validation.Operator = OperatorType.Between;
            validation.Formula1 = "1";
            validation.Formula2 = "10";

            // Doğrulama için iki hücre alanı oluştur
            CellArea area1 = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 1,
                EndColumn = 1
            };  // A1:B2
            CellArea area2 = new CellArea
            {
                StartRow = 2,
                StartColumn = 2,
                EndRow = 3,  // Original code had (2,2,1,1) which would be invalid endRow < startRow
                EndColumn = 3
            };  // C3:D4 (corrected end coordinates)
            
            // Alanları doğrulamaya ekle
            validation.AddArea(area1);
            validation.AddArea(area2);
            Console.WriteLine($"Added areas: {validation.Areas.Length}");

            try
            {
                // Kaldırmak için bir alan içeren dizi oluştur
                CellArea[] removeAreas = { area1 };
                
                // RemoveAreas yöntemini çalıştır
                validation.RemoveAreas(removeAreas);
                Console.WriteLine($"Remaining areas after removal: {validation.Areas.Length}");
                
                // Kalan alanların koordinatlarını göster
                foreach (CellArea remainingArea in validation.Areas)
                {
                    Console.WriteLine($"Area: {remainingArea.StartRow},{remainingArea.StartColumn} to {remainingArea.EndRow},{remainingArea.EndColumn}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("ValidationRemoveAreasDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


