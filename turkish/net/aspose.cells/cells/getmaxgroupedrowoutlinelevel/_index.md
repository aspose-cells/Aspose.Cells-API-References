---
title: "Cells.GetMaxGroupedRowOutlineLevel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. En yüksek gruplanmış satır taslak seviyesini sıfır tabanlı alır"
type: docs
url: /tr/net/aspose.cells/cells/getmaxgroupedrowoutlinelevel/
---
## Cells.GetMaxGroupedRowOutlineLevel method

Maksimum gruplanmış satır anahat seviyesini (sıfır tabanlı) alır.

```csharp
public int GetMaxGroupedRowOutlineLevel()
```

### Dönüş Değeri

En yüksek gruplanmış satır taslak seviyesi (sıfır tabanlı)

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedRowOutlineLevelDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Taslak seviyelerini göstermek için bazı satırları gruplayın
            cells.GroupRows(0, 2, false);
            cells.GroupRows(4, 6, false);
            
            // İç içe gruplanma ekleyin
            cells.GroupRows(4, 5, true);

            // En yüksek gruplanmış satır taslak seviyesini alın
            int maxOutlineLevel = cells.GetMaxGroupedRowOutlineLevel();

            // Sonucu göster
            Console.WriteLine("Maximum grouped row outline level: " + maxOutlineLevel);

            // Her satır için taslak seviyesini göster
            for (int row = 0; row <= 6; row++)
            {
                Console.WriteLine($"Row {row} outline level: {cells.GetGroupedRowOutlineLevel(row)}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


