---
title: "PivotAreaFilter.IsSubtotalSet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotAreaFilter-metod. Hämtar vilken delsumma som är inställd för detta filter"
type: docs
url: /sv/net/aspose.cells.pivot/pivotareafilter/issubtotalset/
---
## PivotAreaFilter.IsSubtotalSet method

Hämtar vilken delsumma som är inställd för detta filter.

```csharp
public bool IsSubtotalSet(PivotFieldSubtotalType subtotalType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Typ av subtotalfunktion. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaFilterMethodIsSubtotalSetWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält och konfigurera delsummor
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields["Category"];
            rowField.IsAutoSubtotals = true;
            rowField.SetSubtotals(PivotFieldSubtotalType.Automatic, true);

            // Skapa pivotområde och kontrollera delsummeinställning
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            
            // Visa hur IsSubtotalSet används
            bool isSubtotalSet = pivotArea.Filters[0].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
            Console.WriteLine($"Is Automatic subtotal set: {isSubtotalSet}");

            // Spara arbetsboken
            workbook.Save("PivotSubtotalDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


