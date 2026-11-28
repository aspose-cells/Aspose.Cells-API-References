---
title: "Cells.SetRowHeightInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Satır yüksekliğini inç biriminde ayarlar"
type: docs
url: /tr/net/aspose.cells/cells/setrowheightinch/
---
## Cells.SetRowHeightInch method

Satır yüksekliğini inç biriminde ayarlar.

```csharp
public void SetRowHeightInch(int row, double inches)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |
| inç | Double | İnç sayısı. 0 ile 409.5/72 arasında olmalıdır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Varsayılan stili ayarla
            Style style = workbook.DefaultStyle;
            style.Font.Name = "Tahoma";
            style.Font.Size = 16;
            style.Font.IsBold = true;
            workbook.DefaultStyle = style;

            // Satır yüksekliklerini inç cinsinden ayarla
            for (int i = 0; i < 10; i++)
            {
                cells.SetRowHeightInch(i, 0.5 + (i * 0.2)); // Demonstrates SetRowHeightInch(Int32, Double)
            }

            // Çalışma kitabını kaydedin
            workbook.Save("RowHeightsInInches.xlsx");
            
            Console.WriteLine("Row heights set successfully in inches.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


