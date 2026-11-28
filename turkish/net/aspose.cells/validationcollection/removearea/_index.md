---
title: "ValidationCollection.RemoveArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ValidationCollection yöntemi. Aralıktaki tüm doğrulama ayarlarını kaldırır"
type: docs
url: /tr/net/aspose.cells/validationcollection/removearea/
---
## ValidationCollection.RemoveArea method

Aralıktaki tüm doğrulama ayarlarını kaldırır..

```csharp
public void RemoveArea(CellArea ca)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | CellArea | Doğrulama ayarlarını içeren aralık. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationCollectionMethodRemoveAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Belirli bir alanda doğrulama oluştur
            ValidationCollection validations = worksheet.Validations;
            CellArea validationArea = CellArea.CreateCellArea(0, 0, 5, 5);
            int validationIndex = validations.Add(validationArea);
            
            // Doğrulamadan kaldırmak için bir alan oluştur
            CellArea removeArea = CellArea.CreateCellArea(2, 2, 4, 4);
            
            try
            {
                // CellArea parametresiyle RemoveArea yöntemini çağır
                validations.RemoveArea(removeArea);
                
                Console.WriteLine("Validation area removed successfully.");
                
                // Kalan doğrulama alanlarını göster
                foreach (Validation validation in validations)
                {
                    if (validation.Areas.Length > 0)
                    {
                        Console.WriteLine($"Remaining validation area: {validation.Areas[0]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("ValidationRemoveAreaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


