---
title: "PivotDateTimeRangeGroupSettings.IsGroupedBy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotDateTimeRangeGroupSettings-Methode. Prüfen, ob das Feld nach dem Typ gruppiert ist"
type: docs
url: /de/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/isgroupedby/
---
## PivotDateTimeRangeGroupSettings.IsGroupedBy method

Überprüft, ob das Feld nach dem Typ gruppiert ist.

```csharp
public bool IsGroupedBy(PivotGroupByType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | PivotGroupByType | Der Gruppentyp |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsMethodIsGroupedByWithPivotGroupByTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Pivot-Tabelle erstellen
            int pivotIndex = worksheet.PivotTables.Add("=A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Felder hinzufügen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Nach Datum gruppieren
            PivotField dateField = pivotTable.RowFields[0];
            DateTime start = new DateTime(2023, 1, 1);
            DateTime end = new DateTime(2023, 12, 31);
            dateField.GroupBy(start, end, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);

            // Gruppierung prüfen
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            bool isGroupedByMonths = groupSettings.IsGroupedBy(PivotGroupByType.Months);
            
            Console.WriteLine($"Is grouped by months: {isGroupedByMonths}");
        }
    }
}
```

### Siehe auch

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


