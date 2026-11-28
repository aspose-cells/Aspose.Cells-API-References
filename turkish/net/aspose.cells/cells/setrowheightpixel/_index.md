---
title: "Cells.SetRowHeightPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Satır yüksekliğini piksel biriminde ayarlar"
type: docs
url: /tr/net/aspose.cells/cells/setrowheightpixel/
---
## Cells.SetRowHeightPixel method

Satır yüksekliğini piksel biriminde ayarlar.

```csharp
public void SetRowHeightPixel(int row, int pixels)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| piksel | Int32 | Piksel sayısı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk satırın yüksekliğini 50 piksele ayarla
            worksheet.Cells.SetRowHeightPixel(0, 50);

            // İkinci satırın yüksekliğini 100 piksele ayarla
            worksheet.Cells.SetRowHeightPixel(1, 100);

            // Çalışma kitabını kaydedin
            workbook.Save("RowHeightPixelDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


