---
title: "ValidationCollection.RemoveACell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ValidationCollection yöntemi. Hücredeki tüm doğrulama ayarlarını kaldırır"
type: docs
url: /tr/net/aspose.cells/validationcollection/removeacell/
---
## ValidationCollection.RemoveACell method

Hücredeki tüm doğrulama ayarlarını kaldırır.

```csharp
public void RemoveACell(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Hücrenin satır indeksi. |
| sütun | Int32 | Hücrenin sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodRemoveACellWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine (satır 0, sütun 0) doğrulama ekle
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            
            Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
            validation.Type = ValidationType.List;
            validation.Formula1 = "Item1,Item2,Item3";

            // A1 hücresinden doğrulamayı kaldır
            worksheet.Validations.RemoveACell(0, 0);

            Console.WriteLine("Validations count after removal: " + worksheet.Validations.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


