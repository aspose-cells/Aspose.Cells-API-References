---
title: "Cells.GetMergedAreas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Tüm birleştirilmiş hücreleri alır"
type: docs
url: /tr/net/aspose.cells/cells/getmergedareas/
---
## Cells.GetMergedAreas method

Tüm birleştirilmiş hücreleri alır.

```csharp
public CellArea[] GetMergedAreas()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMergedAreasDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı birleştirilmiş hücreler oluştur
            worksheet.Cells.Merge(0, 0, 2, 2); // Merge A1:B2
            worksheet.Cells.Merge(3, 3, 3, 2); // Merge D4:E4
            worksheet.Cells.Merge(5, 0, 1, 5); // Merge A6:E6
            
            // Tüm birleştirilmiş alanları al
            CellArea[] mergedAreas = worksheet.Cells.GetMergedAreas();
            
            // Birleştirilmiş alanlar hakkında bilgi göster
            Console.WriteLine("Number of merged areas: " + mergedAreas.Length);
            foreach (CellArea area in mergedAreas)
            {
                Console.WriteLine($"Merged area: StartRow={area.StartRow}, StartColumn={area.StartColumn}, " +
                    $"EndRow={area.EndRow}, EndColumn={area.EndColumn}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


