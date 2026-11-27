---
title: "Class PivotTableCalculateOption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotTableCalculateOption-klass. Representerar alternativen för beräkning av pivottabellens data"
type: docs
url: /sv/net/aspose.cells.pivot/pivottablecalculateoption/
---
## PivotTableCalculateOption class

Representerar alternativen för beräkning av data i pivottabellen.

```csharp
public class PivotTableCalculateOption
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PivotTableCalculateOption](pivottablecalculateoption/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [RefreshCharts](../../aspose.cells.pivot/pivottablecalculateoption/refreshcharts/) { get; set; } | Indikerar om uppdatering av diagram baseras på denna pivottabell. |
| [RefreshData](../../aspose.cells.pivot/pivottablecalculateoption/refreshdata/) { get; set; } | Indikerar om uppdatering av datakällan för pivottabellen. |
| [RefreshOption](../../aspose.cells.pivot/pivottablecalculateoption/refreshoption/) { get; set; } | Hämtar och ställer in alternativ för att uppdatera datakällan till pivotcachen. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/) { get; set; } | Representerar hur man reserverar saknade pivotobjekt. |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionDemo
    {
        public static void PivotTableCalculateOptionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite data för pivåtabellen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Fruit");
            sheet.Cells["B4"].PutValue(70);
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B5"].PutValue(40);

            // Lägg till en pivottabell i kalkylbladet
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Konfigurera pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Skapa ett PivotTableCalculateOption-objekt
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Beräkna pivottabellens data med de angivna alternativen
            pivotTable.CalculateData(calculateOption);

            // Spara arbetsboken
            workbook.Save("PivotTableCalculateOptionExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


