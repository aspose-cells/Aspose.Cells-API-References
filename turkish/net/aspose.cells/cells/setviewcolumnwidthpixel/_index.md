---
title: "Cells.SetViewColumnWidthPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Sütunun genişliğini farklı görünümlerde ayarlar"
type: docs
url: /tr/net/aspose.cells/cells/setviewcolumnwidthpixel/
---
## Cells.SetViewColumnWidthPixel method

Sütunun genişliğini farklı görünümde ayarlar.

```csharp
public void SetViewColumnWidthPixel(int column, int pixels)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |
| piksel | Int32 | Piksel birimindeki genişlik. |

### Açıklamalar

Mevcut görünüm türü PageLayoutView ise, sütunun genişliği yazdırılan genişlikle aynıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetViewColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Örnek veriyi ayarla
            sheet.Cells[0, 0].Value = "Sample Text";

            // Piksel genişliğini hesaplayın (bu örnekte 100 piksel)
            int pixelWidth = 100;

            // Sütun genişliğini piksel olarak ayarlayın
            sheet.Cells.SetViewColumnWidthPixel(0, pixelWidth);

            // Çalışma kitabını kaydedin
            wb.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


