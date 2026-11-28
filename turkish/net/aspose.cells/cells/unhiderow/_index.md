---
title: "Cells.UnhideRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir satırı gizlemeyi kaldırır"
type: docs
url: /tr/net/aspose.cells/cells/unhiderow/
---
## Cells.UnhideRow method

Bir satırı gösterir.

```csharp
public void UnhideRow(int row, double height)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| yükseklik | Double | Satır yüksekliği. Satırın yüksekliği yalnızca satır gizli olduğunda ve verilen yükseklik değeri pozitif olduğunda değişir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır 5'i gizle
            worksheet.Cells.HideRow(5);
            
            // Satır 5'i 12,75 yüksekliğiyle gizlemeyi kaldır
            worksheet.Cells.UnhideRow(5, 12.75);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


