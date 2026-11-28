---
title: "CellsHelper.CellIndexToName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Hücre adını satır ve sütun indekslerine göre alır"
type: docs
url: /tr/net/aspose.cells/cellshelper/cellindextoname/
---
## CellsHelper.CellIndexToName method

Satır ve sütun indekslerine göre hücre adını alır.

```csharp
public static string CellIndexToName(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| sütun | Int32 | Sütun indeksi. |

### Dönüş Değeri

Hücre adı.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCellIndexToNameWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı verileri doldurun
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);

            // Satır ve sütun indekslerinden hücre adını al.
            string cellName = CellsHelper.CellIndexToName(2, 1); // Row 2, Column 1 (B3)

            // Sonucu çıktı olarak ver
            Console.WriteLine("Cell name for row 2, column 1 is: " + cellName);
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


