---
title: "PivotDateTimeRangeGroupSettings.Start"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotDateTimeRangeGroupSettings-Eigenschaft. Gibt das Startdatum und die Startzeit der Gruppe zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/start/
---
## PivotDateTimeRangeGroupSettings.Start property

Ruft das Startdatum‑Uhrzeit der Gruppe ab.

```csharp
public DateTime Start { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsPropertyStartDemo
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

            // Nach Datumsbereich gruppieren
            PivotField dateField = pivotTable.RowFields[0];
            DateTime startDate = new DateTime(2023, 1, 1);
            DateTime endDate = new DateTime(2023, 12, 31);
            dateField.GroupBy(startDate, endDate, new PivotGroupByType[] { PivotGroupByType.Months }, 1, false);

            // Gruppeneinstellungen aufrufen und die Start-Eigenschaft demonstrieren
            PivotDateTimeRangeGroupSettings groupSettings = (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            Console.WriteLine("Group Start Date: " + groupSettings.Start);

            // Arbeitsmappe speichern.
            workbook.Save("PivotDateTimeRangeGroupSettingsStartDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


