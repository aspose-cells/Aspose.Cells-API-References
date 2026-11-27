---
title: "PivotItem.PositionInSameParentNode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotItem‑egenskap. Anger positionsindexet i PivotItems under samma föräldranod"
type: docs
url: /sv/net/aspose.cells.pivot/pivotitem/positioninsameparentnode/
---
## PivotItem.PositionInSameParentNode property

Anger positionsindexet i PivotItems under samma föräldranod.

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int PositionInSameParentNode { get; set; }
```

### Anmärkningar

OBS: Den här metoden är nu föråldrad. Använd istället PivotTable.MoveItem(PivotFieldType, string[],bool,int)-metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyPositionInSameParentNodeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("PivotTest3.xlsx");
            
            // Lägg till ett nytt kalkylblad för pivottabell
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            Worksheet dataSheet = workbook.Worksheets["New Hardware - Yearly"];

            // Lägg till pivottabell
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "PivotTable");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "2014");

            // Konfigurera pivottabell
            PivotField vendorField = pivotTable.RowFields["Vendor"];
            vendorField.SetSubtotals(PivotFieldSubtotalType.None, true);
            pivotTable.ShowColumnGrandTotals = false;

            // Uppdatera och beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Demonstrera egenskapen PositionInSameParentNode
            PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
            
            // Ange positioner inom samma föräldranod
            items["4H12"].PositionInSameParentNode = 1;
            items["DIF400"].PositionInSameParentNode = 2;
            
            // Beräkna om efter att positionerna har ändrats
            pivotTable.CalculateData();
            
            // Ange positioner för en annan grupp
            items["CA32"].PositionInSameParentNode = 1;
            items["AAA3"].PositionInSameParentNode = 2;

            // Spara arbetsboken
            workbook.Save("PivotTableWithPositionInSameParentNode.xlsx");
        }
    }
}
```

### Se även

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


