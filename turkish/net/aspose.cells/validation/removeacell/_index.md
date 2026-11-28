---
title: "Validation.RemoveACell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama yöntemi. Hücredeki doğrulama ayarlarını kaldırın"
type: docs
url: /tr/net/aspose.cells/validation/removeacell/
---
## Validation.RemoveACell method

Hücredeki doğrulama ayarlarını kaldır.

```csharp
public void RemoveACell(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| sütun | Int32 | Sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // İlk hücreye veri doğrulaması ekle
            Validation validation = worksheet.Validations[0];
            validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
            validation.Type = ValidationType.List;
            validation.Formula1 = "1,2,3";
            
            // Doğrulamaya başka bir hücre ekle
            validation.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 1, EndColumn = 1 });
            
            // Doğrulamadan ikinci hücreyi kaldır
            validation.RemoveACell(1, 1);
            
            Console.WriteLine("Cell removed from validation successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


