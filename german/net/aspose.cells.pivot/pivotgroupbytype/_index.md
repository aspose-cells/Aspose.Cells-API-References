---
title: "Enum PivotGroupByType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotGroupByType enum. Stellt den Gruppierungstyp dar"
type: docs
url: /de/net/aspose.cells.pivot/pivotgroupbytype/
---
## PivotGroupByType enumeration

Stellt den Gruppierungs‑Typ dar.

```csharp
[Flags]
public enum PivotGroupByType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| RangeOfValues | `1` | Gruppiere nach Zahlen. |
| Numbers | `1` | Gruppiere nach Zahlen. |
| Seconds | `2` | Stellt den Sekunden‑Gruppierungstyp dar. |
| Minutes | `4` | Präsentiert den Minuten‑Gruppierungstyp. |
| Hours | `8` | Präsentiert den Stunden‑Gruppierungstyp. |
| Days | `10` | Präsentiert den Tages‑Gruppierungstyp. |
| Months | `20` | Präsentiert den Monats‑Gruppierungstyp. |
| Quarters | `40` | Präsentiert den Quartals‑Gruppierungstyp. |
| Years | `80` | Präsentiert den Jahres‑Gruppierungstyp. |
| DateTimes | `FE` | Präsentiert alle Gruppierungstypen von Datums‑ und Zeitwerten. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotGroupByTypeDemo
    {
        public static void PivotGroupByTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Date");
            Style style = workbook.CreateStyle();
            style.Number = 14;//m/d/yyy
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A2"].SetStyle(style);

            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A3"].SetStyle(style);

            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A4"].SetStyle(style);

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Date field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value field

            //TODO
            PivotField dateField = pivotTable.RowFields[0];

            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Years }, 1, false);

            // Zugriff auf die Gruppeneinstellungen
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;

            // Ausgabe der Gruppeneinstellungen
            Console.WriteLine("Group Type: " + groupSettings.Type);
            Console.WriteLine("Start Date: " + groupSettings.Start);
            Console.WriteLine("End Date: " + groupSettings.End);
            Console.WriteLine("Interval: " + groupSettings.Interval);
            Console.WriteLine("Is Grouped By Months: " + groupSettings.IsGroupedBy(PivotGroupByType.Months));

            // Speichere die Arbeitsmappe
            workbook.Save("PivotGroupByTypeExample.xlsx");
            
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


