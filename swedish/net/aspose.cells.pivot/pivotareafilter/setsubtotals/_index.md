---
title: "PivotAreaFilter.SetSubtotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotAreaFilter metod. Delsumma för filtret"
type: docs
url: /sv/net/aspose.cells.pivot/pivotareafilter/setsubtotals/
---
## PivotAreaFilter.SetSubtotals method

Delsumma för filtret.

```csharp
public void SetSubtotals(PivotFieldSubtotalType subtotalType, bool shown)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Delssummafunktionen. |
| visad | Boolean | Indikerar om denna delsumme visas. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaFilterMethodSetSubtotalsWithPivotFieldSubtotalTypeBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            Cells cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 8;

            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("=A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Skapa ett pivotområde med pivottabellparametern
            PivotArea pivotArea = new PivotArea(pivotTable);
            PivotAreaFilter filter = new PivotAreaFilter();

            try
            {
                // Anropa SetSubtotals med Sum-delssummatyp och ange att den ska visas.
                filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
                
                // Verifiera om delsumma är inställd
                bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
                Console.WriteLine($"Sum subtotal is set: {isSumSet}");

                // Uppdatera pivottabellen för att se ändringar
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSubtotals method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("PivotAreaFilterSetSubtotalsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


