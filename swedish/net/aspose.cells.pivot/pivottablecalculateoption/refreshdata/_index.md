---
title: "PivotTableCalculateOption.RefreshData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTableCalculateOption egenskap. Anger om datakällan för pivottabellen ska uppdateras"
type: docs
url: /sv/net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

Indikerar om uppdatering av datakällan för pivottabellen.

```csharp
public bool RefreshData { get; set; }
```

### Anmärkningar

Om den är sann, uppdatera pivot cache från datakällan, sedan beräkna alla pivottabeller baserat på samma pivot cache.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyRefreshDataDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ställ in exempeldata för pivottabell
            var cells = sheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("A");
            cells["B2"].PutValue(100);
            cells["A3"].PutValue("B");
            cells["B3"].PutValue(200);
            cells["A4"].PutValue("C");
            cells["B4"].PutValue(300);

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ändra källdata
            cells["B2"].PutValue(150); // Change value from 100 to 150

            // Beräkna pivottabell med RefreshData-alternativet
            PivotTableCalculateOption options = new PivotTableCalculateOption();
            options.RefreshData = true;
            pivotTable.CalculateData(options);

            // Skriv ut det uppdaterade pivottabellvärdet
            Console.WriteLine("Updated Pivot Table Value: " + cells["F5"].StringValue);
        }
    }
}
```

### Se även

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


