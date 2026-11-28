---
title: "Worksheet.Timelines"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasındaki Timeline koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/worksheet/timelines/
---
## Worksheet.Timelines property

Çalışma sayfasındaki Timeline koleksiyonunu al.

```csharp
public TimelineCollection Timelines { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTimelinesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Özet tablo için örnek veri ekle
            sheet.Cells["A1"].Value = "Ship Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 1, 15);
            sheet.Cells["A4"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // Özet tablo oluştur
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Ship Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Özet tablo için zaman çizelgesi kontrolü ekleyin
            sheet.Timelines.Add(pivotTable, 0, 0, "Ship Date");

            // Çalışma kitabını kaydedin
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TimelineCollection](../../../aspose.cells.timelines/timelinecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


