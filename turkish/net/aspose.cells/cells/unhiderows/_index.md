---
title: "Cells.UnhideRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Gizli satırları ortaya çıkarır"
type: docs
url: /tr/net/aspose.cells/cells/unhiderows/
---
## Cells.UnhideRows method

Gizli satırları gösterir.

```csharp
public void UnhideRows(int row, int totalRows, double height)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| totalRows | Int32 | Satır numarası. |
| yükseklik | Double | Satır yüksekliği. Satırın yüksekliği yalnızca satır gizli olduğunda ve verilen yükseklik değeri pozitif olduğunda değişir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Satır 0-4'ü gizle
            cells.HideRows(0, 5);
            
            // Satır 0-4'ü yükseklik ayarıyla ortaya çıkar (-1 otomatik sığdırma için)
            cells.UnhideRows(0, 5, -1);
            
            // Satırların ortaya çıkarıldığını doğrula
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Row {i} hidden status: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


