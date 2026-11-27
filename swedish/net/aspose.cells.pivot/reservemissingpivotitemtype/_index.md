---
title: "Enum ReserveMissingPivotItemType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.ReserveMissingPivotItemType enum. Representerar hur man behåller de saknade pivotelementen"
type: docs
url: /sv/net/aspose.cells.pivot/reservemissingpivotitemtype/
---
## ReserveMissingPivotItemType enumeration

Representerar hur man behåller de saknade pivotobjekten.

```csharp
public enum ReserveMissingPivotItemType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `0` | Tar bort gamla saknade pivotelement och reserverar borttagna element från den nya datakällan som saknade element. |
| All | `1` | Reserverar alla saknade objekt. |
| None | `2` | Tar bort alla saknade pivotelement. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class ReserveMissingPivotItemTypeDemo
    {
        public static void ReserveMissingPivotItemTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Lägg till ett nytt kalkylblad i arbetsboken
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till en pivottabell i kalkylbladet
            int pivotTableIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Ställ in alternativet ReserveMissingPivotItemType
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Beräkna pivottabellen med de angivna alternativen
            pivotTable.CalculateData(calculateOption);

            // Uppdatera pivottabellen
            pivotTable.RefreshData();

            // Spara arbetsboken
            workbook.Save("ReserveMissingPivotItemTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


