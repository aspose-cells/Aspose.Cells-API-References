---
title: "Cells.GetRowHeightPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen bir satırın yüksekliğini piksel biriminde alır"
type: docs
url: /tr/net/aspose.cells/cells/getrowheightpixel/
---
## Cells.GetRowHeightPixel method

Belirtilen bir satırın yüksekliğini piksel biriminde alır.

```csharp
public int GetRowHeightPixel(int row)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi |

### Dönüş Değeri

Satır yüksekliği

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetRowHeightPixelWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir Workbook örneği oluşturun
            Workbook wb = new Workbook();

            // İlk çalışma sayfasını al
            Worksheet worksheet = wb.Worksheets[0];

            // Satır 5 için satır yüksekliğini ayarla (piksel olarak)
            worksheet.Cells.SetRowHeightPixel(5, 30);

            // Satır 5 için satır yüksekliğini al (piksel olarak)
            int rowHeight = worksheet.Cells.GetRowHeightPixel(5);

            Console.WriteLine("Row height of row 5 in pixels: " + rowHeight);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


