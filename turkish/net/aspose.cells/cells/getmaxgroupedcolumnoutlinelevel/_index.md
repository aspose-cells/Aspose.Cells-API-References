---
title: "Cells.GetMaxGroupedColumnOutlineLevel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Sıfır tabanlı en yüksek gruplanmış sütun anahat seviyesini alır"
type: docs
url: /tr/net/aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/
---
## Cells.GetMaxGroupedColumnOutlineLevel method

Maksimum gruplanmış sütun anahat seviyesini (sıfır tabanlı) alır.

```csharp
public int GetMaxGroupedColumnOutlineLevel()
```

### Dönüş Değeri

En yüksek gruplanmış sütun anahat seviyesi (sıfır tabanlı)

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedColumnOutlineLevelDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Anahat seviyelerini göstermek için bazı sütunları grupla
            cells.GroupColumns(0, 2, false);
            cells.GroupColumns(3, 5, false);
            
            // En yüksek gruplanmış sütun anahat seviyesini al
            int maxOutlineLevel = cells.GetMaxGroupedColumnOutlineLevel();
            
            Console.WriteLine("Maximum grouped column outline level: " + maxOutlineLevel);
            
            // Her sütun için anahat seviyesini göster
            for (int col = 0; col < 6; col++)
            {
                int outlineLevel = cells.GetGroupedColumnOutlineLevel(col);
                Console.WriteLine($"Column {col} outline level: {outlineLevel}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("GroupedColumnsOutlineLevel.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


