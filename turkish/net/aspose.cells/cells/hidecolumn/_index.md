---
title: "Cells.HideColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir sütunu gizler"
type: docs
url: /tr/net/aspose.cells/cells/hidecolumn/
---
## Cells.HideColumn method

Bir sütunu gizler.

```csharp
public void HideColumn(int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Gizleyeceğimiz sütunda bazı veriler ayarla
            cells["B1"].PutValue("This column will be hidden");
            cells["B2"].PutValue(123.45);

            // Sütun B'yi (indeks 1) gizle
            cells.HideColumn(1);

            // Standart genişlikteki sütunu göster
            cells.UnhideColumn(1, cells.StandardWidth);

            // Çalışma kitabını kaydedin
            workbook.Save("HideColumnDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


