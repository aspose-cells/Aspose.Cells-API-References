---
title: "Cells.GetGroupedRowOutlineLevel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Satırın sıfır tabanlı taslak seviyesini alır"
type: docs
url: /tr/net/aspose.cells/cells/getgroupedrowoutlinelevel/
---
## Cells.GetGroupedRowOutlineLevel method

Satırın anahat seviyesini (sıfır tabanlı) alır.

```csharp
public int GetGroupedRowOutlineLevel(int rowIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | Int32 | Satır indeksi. |

### Dönüş Değeri

Satırın taslak seviyesi (sıfır tabanlı).

### Açıklamalar

Satır gruplanmamışsa, sıfır döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedRowOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Satırları 0-3 gruplandır (seviye 1)
            cells.GroupRows(0, 3, false);
            
            // Satırları 0-1 gruplandır (seviye 2)
            cells.GroupRows(0, 1, false);

            // Her satır için taslak seviyesini al
            for (int row = 0; row <= 4; row++)
            {
                int outlineLevel = cells.GetGroupedRowOutlineLevel(row);
                Console.WriteLine($"Row {row} outline level: {outlineLevel}");
            }

            // Tüm satırların grubunu kaldır
            cells.UngroupRows(0, 3);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


