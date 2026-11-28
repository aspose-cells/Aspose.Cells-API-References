---
title: "Cells.SetColumnWidthInch"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Normal görünümde sütun genişliğini inç biriminde ayarlar."
type: docs
url: /tr/net/aspose.cells/cells/setcolumnwidthinch/
---
## Cells.SetColumnWidthInch method

Normal görünümde sütun genişliğini inç biriminde ayarlar.

```csharp
public void SetColumnWidthInch(int column, double inches)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |
| inç | Double | İnç sayısı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sütun genişliklerini inç cinsinden ayarlayın.
            cells.SetColumnWidthInch(0, 2.0);
            cells.SetColumnWidthInch(1, 1.5);
            cells.SetColumnWidthInch(2, 0.8);

            // Dosyanın görünür olması için hücrelere bazı veriler ekleyin.
            cells["A1"].PutValue("Column A (2 inches)");
            cells["B1"].PutValue("Column B (1.5 inches)");
            cells["C1"].PutValue("Column C (0.8 inches)");

            // Çalışma kitabını kaydedin
            workbook.Save("ColumnWidthsInInches.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


