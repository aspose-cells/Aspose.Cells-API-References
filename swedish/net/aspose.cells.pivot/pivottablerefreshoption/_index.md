---
title: "Klass PivotTableRefreshOption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotTableRefreshOption-klass. Representerar alternativen för att uppdatera datakällan för pivottabellen."
type: docs
url: /sv/net/aspose.cells.pivot/pivottablerefreshoption/
---
## PivotTableRefreshOption class

Representerar alternativen för att uppdatera datakällan för pivottabellen.

```csharp
public class PivotTableRefreshOption
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PivotTableRefreshOption](pivottablerefreshoption/)() | Representerar alternativen för att uppdatera datakällan för pivottabellen. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [IsKeepOriginalOrder](../../aspose.cells.pivot/pivottablerefreshoption/iskeeporiginalorder/) { get; set; } | Anger om pivotobjektens ursprungliga ordning ska behållas som i den gamla datakällan. |
| [KeepCachedLocalGroupData](../../aspose.cells.pivot/pivottablerefreshoption/keepcachedlocalgroupdata/) { get; set; } | Anger om cachad lokal gruppdata ska behållas om de maximala och minimala värdena förblir oförändrade. Standardvärdet är false, vilket betyder att gruppen uppdateras med lokala inställningar. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablerefreshoption/reservemissingpivotitemtype/) { get; set; } | Representerar hur man reserverar saknade pivotobjekt. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableRefreshOptionDemo
    {
        public static void PivotTableRefreshOptionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Lägg till en pivottabell i kalkylbladet
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Skapa en instans av PivotTableRefreshOption
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Uppdatera pivottabellen med de angivna alternativen
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotTableRefreshOptionExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


