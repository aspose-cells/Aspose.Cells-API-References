---
title: "Cells.HideRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Birden fazla satırı gizler"
type: docs
url: /tr/net/aspose.cells/cells/hiderows/
---
## Cells.HideRows method

Birden fazla satırı gizler.

```csharp
public void HideRows(int row, int totalRows)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| totalRows | Int32 | Satır numarası. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı verileri doldurun
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i+1}, Col {j+1}";
                }
            }

            // 3 ila 5 satırları gizle (sıfır tabanlı indeks: 2 ila 4)
            worksheet.Cells.HideRows(2, 3);

            // Çalışma kitabını kaydedin
            workbook.Save("HideRowsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


