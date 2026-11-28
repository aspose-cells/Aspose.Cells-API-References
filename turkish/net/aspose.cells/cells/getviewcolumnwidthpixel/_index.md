---
title: "Cells.GetViewColumnWidthPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Farklı görünüm tipinde genişliği al"
type: docs
url: /tr/net/aspose.cells/cells/getviewcolumnwidthpixel/
---
## Cells.GetViewColumnWidthPixel method

Farklı görünüm tipinde genişliği al.

```csharp
public int GetViewColumnWidthPixel(int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |

### Dönüş Değeri

piksel biriminde sütun genişliği

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Görünüm tipini PageLayoutView olarak ayarla
            worksheet.ViewType = ViewType.PageLayoutView;
            
            // Sütun genişliğini karakter cinsinden ayarlayın (piksellere dönüştürülecek)
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // Sütun genişliğini piksel olarak al
            int columnWidthInPixels = worksheet.Cells.GetViewColumnWidthPixel(0);
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Column width in pixels: " + columnWidthInPixels);
            
            // Çalışma kitabını kaydedin
            workbook.Save("ColumnWidthTest.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


