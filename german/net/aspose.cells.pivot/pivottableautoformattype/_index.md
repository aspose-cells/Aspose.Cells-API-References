---
title: "Aufzählung PivotTableAutoFormatType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotTableAutoFormatType enum. Stellt den Autoformattyp der PivotTable dar."
type: docs
url: /de/net/aspose.cells.pivot/pivottableautoformattype/
---
## PivotTableAutoFormatType enumeration

Stellt den automatischen Formattyp einer PivotTable dar.

```csharp
public enum PivotTableAutoFormatType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Stellt den Formattyp None dar. |
| Classic | `1` | Stellt den klassischen Autoformattyp dar. |
| Report1 | `2` | Stellt den Formattyp Report1 dar. |
| Report2 | `3` | Stellt den Formattyp Report2 dar. |
| Report3 | `4` | Stellt den Formattyp Report3 dar. |
| Report4 | `5` | Stellt den Formattyp Report4 dar. |
| Report5 | `6` | Stellt den Formattyp Report5 dar. |
| Report6 | `7` | Stellt den Formattyp Report6 dar. |
| Report7 | `8` | Stellt den Formattyp Report7 dar. |
| Report8 | `9` | Stellt den Formattyp Report8 dar. |
| Report9 | `10` | Stellt den Formattyp Report9 dar. |
| Report10 | `11` | Stellt den Formattyp Report10 dar. |
| Table1 | `12` | Stellt den Formattyp Table1 dar. |
| Table2 | `13` | Stellt den Formattyp Table2 dar. |
| Table3 | `14` | Stellt den Formattyp Table3 dar. |
| Table4 | `15` | Stellt den Formattyp Table4 dar. |
| Table5 | `16` | Stellt den Formattyp Table5 dar. |
| Table6 | `17` | Stellt den Formattyp Table6 dar. |
| Table7 | `18` | Stellt den Formattyp Table7 dar. |
| Table8 | `19` | Stellt den Formattyp Table8 dar. |
| Table9 | `20` | Stellt den Formattyp Table9 dar. |
| Table10 | `21` | Stellt den Formattyp Table10 dar. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten für die PivotTable hinzu
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

            // Füge eine PivotTable zum Arbeitsblatt hinzu
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Felder zur PivotTable hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Legen Sie den automatischen Formattyp für die PivotTable fest
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report1;

            // Speichere die Arbeitsmappe
            workbook.Save("PivotTableAutoFormatTypeExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


