---
title: "PivotTable.RefreshDataOnOpeningFile"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable egenskap. Anger om data ska uppdateras när filen öppnas"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/refreshdataonopeningfile/
---
## PivotTable.RefreshDataOnOpeningFile property

Anger om data ska uppdateras vid öppning av filen.

```csharp
public bool RefreshDataOnOpeningFile { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRefreshDataOnOpeningFileDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Banana";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Orange";
            cells["B4"].Value = 3000;

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ange RefreshDataOnOpeningFile egenskap
            pivotTable.RefreshDataOnOpeningFile = false;

            // Spara arbetsboken
            workbook.Save("PivotTableRefreshDataOnOpeningFileDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


