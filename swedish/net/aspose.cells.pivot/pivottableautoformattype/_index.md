---
title: "Enum PivotTableAutoFormatType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotTableAutoFormatType enum. Representerar PivotTable autoformattyp"
type: docs
url: /sv/net/aspose.cells.pivot/pivottableautoformattype/
---
## PivotTableAutoFormatType enumeration

Representerar PivotTable‑autoformattyp.

```csharp
public enum PivotTableAutoFormatType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Representerar Ingen formattyp. |
| Classic | `1` | Representerar Classic formattyp. |
| Report1 | `2` | Representerar Report1 formattyp. |
| Report2 | `3` | Representerar Report2 formattyp. |
| Report3 | `4` | Representerar Report3 formattyp. |
| Report4 | `5` | Representerar Report4 formattyp. |
| Report5 | `6` | Representerar Report5 formattyp. |
| Report6 | `7` | Representerar Report6 formattyp. |
| Report7 | `8` | Representerar Report7 formattyp. |
| Report8 | `9` | Representerar Report8 formattyp. |
| Report9 | `10` | Representerar Report9 formattyp. |
| Report10 | `11` | Representerar Report10 formattyp. |
| Table1 | `12` | Representerar Table1 formattyp. |
| Table2 | `13` | Representerar Table2 formattyp. |
| Table3 | `14` | Representerar Table3 formattyp. |
| Table4 | `15` | Representerar Table4 formattyp. |
| Table5 | `16` | Representerar Table5 formattyp. |
| Table6 | `17` | Representerar Table6 formattyp. |
| Table7 | `18` | Representerar Table7 formattyp. |
| Table8 | `19` | Representerar Table8 formattyp. |
| Table9 | `20` | Representerar Table9 formattyp. |
| Table10 | `21` | Representerar Table10 formattyp. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableAutoFormatTypeDemo
    {
        public static void PivotTableAutoFormatTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för PivotTable
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Lägg till en pivottabell i kalkylbladet
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Ställ in autoformattypen för PivotTable
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report1;

            // Spara arbetsboken
            workbook.Save("PivotTableAutoFormatTypeExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


