---
title: "Cells.SetRowHeight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen satırın yüksekliğini ayarlar"
type: docs
url: /tr/net/aspose.cells/cells/setrowheight/
---
## Cells.SetRowHeight method

Belirtilen satırın yüksekliğini ayarlar.

```csharp
public void SetRowHeight(int row, double height)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| yükseklik | Double | Satır yüksekliği. Birim olarak puan kullanılır. 0 ile 409.5 arasında olmalıdır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // İlk satırın (indeks 0) yüksekliğini 25.5 puana ayarlayın
            cells.SetRowHeight(0, 25.5);

            // Satır yüksekliğini doğrulayın
            Console.WriteLine("Row height of row 0: " + cells.GetRowHeight(0));
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


