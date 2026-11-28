---
title: "ValidationCollection.GetValidationInCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ValidationCollection yöntemi. Belirtilen hücreye uygulanan doğrulamayı alır"
type: docs
url: /tr/net/aspose.cells/validationcollection/getvalidationincell/
---
## ValidationCollection.GetValidationInCell method

Verilen hücreye uygulanan doğrulamayı alır.

```csharp
public Validation GetValidationInCell(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| sütun | Int32 | Sütun indeksi. |

### Dönüş Değeri

Verilen hücrede doğrulama yoksa bir [`Validation`](../../validation/) nesnesi veya null döndürür

### Örnekler

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodGetValidationInCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine (0,0) veri doğrulaması ekle
            Validation validation = worksheet.Validations[worksheet.Validations.Add()];
            validation.Type = ValidationType.List;
            validation.Formula1 = "\"Option1,Option2,Option3\"";
            
            // StartRow, StartColumn, EndRow, EndColumn ile CellArea oluştur
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 0;
            area.EndColumn = 0;
            validation.AddArea(area);

            // A1 hücresinden (0,0) doğrulamayı al
            Validation validationInCell = worksheet.Validations.GetValidationInCell(0, 0);
            
            if (validationInCell != null && validationInCell.Type == ValidationType.List)
            {
                Console.WriteLine("Cell A1 has list validation with formula: " + validationInCell.Formula1);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


