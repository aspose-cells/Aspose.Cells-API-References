---
title: "Enum PivotFieldSubtotalType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotFieldSubtotalType enum. Sammanfattande beskrivning för PivotFieldSubtotalType"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldsubtotaltype/
---
## PivotFieldSubtotalType enumeration

Sammanfattande beskrivning för PivotFieldSubtotalType.

```csharp
[Flags]
public enum PivotFieldSubtotalType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Representerar ingen delsumme-typ. |
| Automatic | `1` | Representerar automatisk delsumme-typ. |
| Sum | `2` | Representerar sum-delsummatyp. |
| Count | `4` | Representerar räkne-delsummatyp. |
| Average | `8` | Representerar medelvärdes-delsummatyp. |
| Max | `10` | Representerar max-delsummatyp. |
| Min | `20` | Representerar min-delsummatyp. |
| Product | `40` | Representerar produkt-delsummatyp. |
| CountNums | `80` | Representerar antal-nummer-delsummatyp. |
| Stdev | `100` | Representerar standardavvikelse-delsummatyp. |
| Stdevp | `200` | Representerar standardavvikelse för en population-delsummatyp. |
| Var | `400` | Representerar varians-delsummatyp. |
| Varp | `800` | Representerar varians för en population-delsummatyp. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldSubtotalTypeDemo
    {
        public static void PivotFieldSubtotalTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;

            // Lägg till en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Ange delsumme-typ för radfältet
            PivotField rowField = pivotTable.RowFields[0];
            rowField.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            rowField.SetSubtotals(PivotFieldSubtotalType.Count, true);

            // Uppdatera och beräkna pivottabellens data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotFieldSubtotalTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


