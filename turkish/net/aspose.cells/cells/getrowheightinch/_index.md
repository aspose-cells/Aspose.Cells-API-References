---
title: "Cells.GetRowHeightInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen bir satırın yüksekliğini inç biriminde alır"
type: docs
url: /tr/net/aspose.cells/cells/getrowheightinch/
---
## Cells.GetRowHeightInch method

Belirtilen bir satırın yüksekliğini inç biriminde alır.

```csharp
public double GetRowHeightInch(int row)
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
    public class CellsMethodGetRowHeightInchWithInt32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Satır 5 için satır yüksekliğini inç cinsinden ayarla
            cells.SetRowHeightInch(5, 1.5);

            // Satır 5 için satır yüksekliğini inç cinsinden al
            double rowHeight = cells.GetRowHeightInch(5);

            // Sonucu çıktı olarak ver
            Console.WriteLine("Row height in inches: " + rowHeight);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


