---
title: "Row.GroupLevel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row özelliği. Satırın grup seviyesini alır"
type: docs
url: /tr/net/aspose.cells/row/grouplevel/
---
## Row.GroupLevel property

Satırın grup seviyesini alır.

```csharp
public byte GroupLevel { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Satırları 4-6 grupla (gizli = false)
            worksheet.Cells.GroupRows(3, 5, false);

            // Satır 4'ün grup seviyesine eriş
            int groupLevel = worksheet.Cells.Rows[3].GroupLevel;
            Console.WriteLine("Group level of row 4: " + groupLevel);

            // Satırların grubunu çöz
            worksheet.Cells.UngroupRows(3, 5);
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


