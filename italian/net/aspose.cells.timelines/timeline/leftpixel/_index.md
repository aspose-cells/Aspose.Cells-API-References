---
title: "Timeline.LeftPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Timeline. Restituisce o imposta lo spostamento orizzontale della forma della timeline dalla sua colonna sinistra in pixel"
type: docs
url: /it/net/aspose.cells.timelines/timeline/leftpixel/
---
## Timeline.LeftPixel property

Restituisce o imposta lo spostamento orizzontale della forma della timeline dalla sua colonna sinistra, in pixel.

```csharp
[Obsolete("Use Shape.Left property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int LeftPixel { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Left. Questa proprietà sarà rimossa 12 mesi dopo, a partire da maggio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyLeftPixelDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].Value = "Date";
            sheet.Cells["A2"].Value = new DateTime(2023, 1, 1);
            sheet.Cells["A3"].Value = new DateTime(2023, 2, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;

            // Crea tabella pivot
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();

            // Aggiungi una timeline e ottienila dalla collezione
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Dimostra la proprietà LeftPixel
            timeline.LeftPixel = 150;
            timeline.TopPixel = 50;
            timeline.WidthPixel = 200;
            timeline.HeightPixel = 80;

            // Salva cartella di lavoro
            workbook.Save("TimelineLeftPixelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


