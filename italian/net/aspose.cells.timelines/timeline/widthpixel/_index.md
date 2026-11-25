---
title: "Timeline.WidthPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Timeline. Restituisce o imposta la larghezza della timeline specificata in pixel"
type: docs
url: /it/net/aspose.cells.timelines/timeline/widthpixel/
---
## Timeline.WidthPixel property

Restituisce o imposta la larghezza della timeline specificata, in pixel.

```csharp
[Obsolete("Use Shape.Width property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int WidthPixel { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Width. Questa proprietà sarà rimossa 12 mesi dopo, a partire da maggio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Timelines;

namespace AsposeCellsExamples
{
    public class TimelinePropertyWidthPixelDemo
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
            sheet.Cells["A4"].Value = new DateTime(2023, 3, 1);
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 1000;
            sheet.Cells["B3"].Value = 2000;
            sheet.Cells["B4"].Value = 3000;

            // Crea tabella pivot e ottieni il riferimento
            int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Date");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivot.RefreshData();
            pivot.CalculateData();

            // Aggiungi timeline e ottieni il riferimento
            int timelineIndex = sheet.Timelines.Add(pivot, 0, 0, "Date");
            Timeline timeline = sheet.Timelines[timelineIndex];
            
            // Imposta le proprietà della timeline includendo WidthPixel
            timeline.WidthPixel = 300;
            timeline.HeightPixel = 100;
            timeline.Caption = "Sales Timeline";

            // Salva la cartella di lavoro
            workbook.Save("TimelineWidthPixelDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Timeline](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)


