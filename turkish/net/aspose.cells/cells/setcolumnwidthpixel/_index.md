---
title: "Cells.SetColumnWidthPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Normal görünümde sütun genişliğini piksel biriminde ayarlar"
type: docs
url: /tr/net/aspose.cells/cells/setcolumnwidthpixel/
---
## Cells.SetColumnWidthPixel method

Normal görünümde sütun genişliğini piksel biriminde ayarlar.

```csharp
public void SetColumnWidthPixel(int column, int pixels)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |
| piksel | Int32 | Piksel sayısı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // 1'den 5'e kadar sütunlar için sütun genişliklerini piksel cinsinden ayarlayın
            for (int i = 0; i < 5; i++)
            {
                cells.SetColumnWidthPixel(i, 120); // 120 pixels width
            }

            // Çalışma kitabını kaydedin
            workbook.Save("SetColumnWidthPixelDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


