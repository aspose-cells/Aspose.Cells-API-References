---
title: "Cells.GetDependents"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirli bir hücreye referans veren tüm hücreleri al"
type: docs
url: /tr/net/aspose.cells/cells/getdependents/
---
## Cells.GetDependents method

Belirli hücreye referans veren tüm hücreleri al.

```csharp
public Cell[] GetDependents(bool isAll, int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isAll | Boolean | Diğer çalışma sayfalarının kontrol edilip edilmediğini belirtir |
| satır | Int32 | Satır indeksi. |
| sütun | Int32 | Sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetDependentsWithBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek formüller ve değerleri ayarlayın
            cells["A1"].PutValue(10);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=A1+B1";
            cells["D1"].Formula = "=B1*3";
            cells["F4"].Formula = "=A1*5";

            // Formülleri hesapla
            workbook.CalculateFormula();

            // A1 hücresinin (satır 0, sütun 0) doğrudan bağımlılarını alın
            Cell[] directDependents = cells.GetDependents(false, 0, 0);
            Console.WriteLine("Direct dependents of A1:");
            foreach (Cell cell in directDependents)
            {
                Console.WriteLine(cell.Name);
            }

            // A1 hücresinin (satır 0, sütun 0) tüm bağımlılarını (dolaylı olanlar dahil) alın
            Cell[] allDependents = cells.GetDependents(true, 0, 0);
            Console.WriteLine("\nAll dependents of A1:");
            foreach (Cell cell in allDependents)
            {
                Console.WriteLine(cell.Name);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


