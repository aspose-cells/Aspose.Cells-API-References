---
title: "PivotTableCalculateOption.ReserveMissingPivotItemType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTableCalculateOption-egenskap. Representerar hur man reserverar saknade pivotobjekt"
type: docs
url: /sv/net/aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/
---
## PivotTableCalculateOption.ReserveMissingPivotItemType property

Representerar hur man reserverar saknade pivotobjekt.

```csharp
public ReserveMissingPivotItemType ReserveMissingPivotItemType { get; set; }
```

### Anmärkningar

Fungerar endast när [`RefreshData`](../refreshdata/) är sann.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyReserveMissingPivotItemTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("A");
            sheet.Cells["B4"].PutValue(30);

            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Konfigurera pivottfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Ställ in beräkningsalternativ med ReserveMissingPivotItemType
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Beräkna med alternativ
            pivotTable.CalculateData(options);

            // Spara resultatet
            workbook.Save("PivotTableReserveMissingItemsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ReserveMissingPivotItemType](../../reservemissingpivotitemtype/)
* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


