---
title: "Klass PivotAreaFilter"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotAreaFilter-klass. Representerar filtret för PivotArea för PivotTable"
type: docs
url: /sv/net/aspose.cells.pivot/pivotareafilter/
---
## PivotAreaFilter class

Representerar filtret för [`PivotArea`](../pivotarea/) för [`PivotTable`](../pivottable/).

```csharp
public class PivotAreaFilter
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PivotAreaFilter](pivotareafilter/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FieldIndex](../../aspose.cells.pivot/pivotareafilter/fieldindex/) { get; } | Hämtar indexet för fältet i källfälten som detta filter refererar till. Ett värde på -2 indikerar värdefältet. |
| [Selected](../../aspose.cells.pivot/pivotareafilter/selected/) { get; set; } | Indikerar om detta fält har markering. Fungerar endast när pivottabellen är i översiktsvy. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [IsSubtotalSet](../../aspose.cells.pivot/pivotareafilter/issubtotalset/)(PivotFieldSubtotalType) | Hämtar vilken delsumma som är inställd för detta filter. |
| [SetSubtotals](../../aspose.cells.pivot/pivotareafilter/setsubtotals/)(PivotFieldSubtotalType, bool) | Delsumma för filtret. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Exempel på datauppsättning
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            
            // Skapa pivottabell – fixa hantering av returvärde
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Skapa och konfigurera PivotAreaFilter
            PivotAreaFilter filter = new PivotAreaFilter();
            filter.Selected = true;
            filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            
            // Demonstrera metoder
            bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
            Console.WriteLine($"Sum subtotal visibility set: {isSumSet}");
            
            workbook.Save("PivotAreaFilterDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


