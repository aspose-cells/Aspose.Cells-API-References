---
title: "Enum PivotFieldType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotFieldType enum. Representerar fälttyp för pivottabell"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldtype/
---
## PivotFieldType enumeration

Representerar PivotTable-fälttyp.

```csharp
public enum PivotFieldType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Undefined | `0` | Visar grundläggande pivot-fälttyp. |
| Row | `1` | Visar rad-pivot-fälttyp. |
| Column | `2` | Visar kolumn-pivot-fälttyp. |
| Page | `4` | Visar sid-pivot-fälttyp. |
| Data | `8` | Visar data-pivot-fälttyp. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldTypeDemo
    {
        public static void PivotFieldTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Grape";
            worksheet.Cells[2, 0].Value = "Blueberry";
            worksheet.Cells[3, 0].Value = "Kiwi";
            worksheet.Cells[4, 0].Value = "Cherry";
            worksheet.Cells[5, 0].Value = "Grape";
            worksheet.Cells[6, 0].Value = "Blueberry";
            worksheet.Cells[7, 0].Value = "Kiwi";
            worksheet.Cells[8, 0].Value = "Cherry";

            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[4, 1].Value = 2020;
            worksheet.Cells[5, 1].Value = 2021;
            worksheet.Cells[6, 1].Value = 2021;
            worksheet.Cells[7, 1].Value = 2021;
            worksheet.Cells[8, 1].Value = 2021;

            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 2].Value = 80;
            worksheet.Cells[5, 2].Value = 90;
            worksheet.Cells[6, 2].Value = 100;
            worksheet.Cells[7, 2].Value = 110;
            worksheet.Cells[8, 2].Value = 120;

            // Lägg till en pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:C9", "A12", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Ställ in pivottabellens stil
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;

            // Uppdatera och beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotFieldTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


