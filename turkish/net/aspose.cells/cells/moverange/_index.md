---
title: "Cells.MoveRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Aralığı taşır"
type: docs
url: /tr/net/aspose.cells/cells/moverange/
---
## Cells.MoveRange method

Aralığı taşır.

```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceArea | CellArea | Taşınması gereken aralık. |
| destRow | Int32 | Hedef satır. |
| destColumn | Int32 | Hedef sütun. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMoveRangeWithCellAreaInt32Int32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücrelere değerleri koy
            cells["A1"].PutValue("Original");
            cells["B1"].PutValue(100);
            cells["A2"].PutValue("Data");
            cells["B2"].PutValue(200);

            // Taşınacak hücre alanını tanımlayın (A1:B2)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 1;
            area.EndColumn = 1;

            // Aralığı 2 satır aşağı ve 3 sütun sağa taşıyın
            cells.MoveRange(area, 2, 3);

            // Çalışma kitabını kaydedin
            workbook.Save("MoveRangeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


