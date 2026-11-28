---
title: "Cells.GetViewRowHeight"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen bir satırın yüksekliğini alır"
type: docs
url: /tr/net/aspose.cells/cells/getviewrowheight/
---
## Cells.GetViewRowHeight method

Belirtilen bir satırın yüksekliğini alır.

```csharp
public double GetViewRowHeight(int row)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |

### Dönüş Değeri

Satır yüksekliği.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewRowHeightWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır 3 için satır yüksekliğini ayarla (puan cinsinden)
            worksheet.Cells.SetRowHeight(3, 15);
            
            // Satır 3 için görüntü satır yüksekliğini al
            double viewRowHeight = worksheet.Cells.GetViewRowHeight(3);
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("View Row Height for row 3: " + viewRowHeight);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


