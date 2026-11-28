---
title: "Cells.GetGroupedColumnOutlineLevel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells metodu. Sütunun sıfır tabanlı taslak seviyesini alır"
type: docs
url: /tr/net/aspose.cells/cells/getgroupedcolumnoutlinelevel/
---
## Cells.GetGroupedColumnOutlineLevel method

Sütunun anahat seviyesini (sıfır tabanlı) alır.

```csharp
public int GetGroupedColumnOutlineLevel(int columnIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | Int32 | Sütun indeksi |

### Dönüş Değeri

Sütunun taslak seviyesi

### Açıklamalar

Sütun gruplanmamışsa, sıfır döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedColumnOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sütunları (ilk 3 sütun) gizlemeden grupla
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // İlk sütunun anahat seviyesini al
            int outlineLevel = worksheet.Cells.GetGroupedColumnOutlineLevel(0);
            
            Console.WriteLine("Outline level of column 0: " + outlineLevel);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


