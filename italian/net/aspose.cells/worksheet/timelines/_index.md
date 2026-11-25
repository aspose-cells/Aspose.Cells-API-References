---
title: "Worksheet.Timelines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Ottieni la raccolta Timeline nel foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/timelines/
---
## Worksheet.Timelines property

Ottieni la collezione di Timeline nel foglio di lavoro

```csharp
public TimelineCollection Timelines { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per la tabella pivot
            sheet.Cells["A1"].Value = "Ship Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 1, 15);
            sheet.Cells["A4"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Ship Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Aggiungi il controllo timeline per la tabella pivot
            sheet.Timelines.Add(pivotTable, 0, 0, "Ship Date");

            // Salva la cartella di lavoro
            workbook.Save("TimelineDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TimelineCollection](../../../aspose.cells.timelines/timelinecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


