---
title: "PivotDateTimeRangeGroupSettings.Interval"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotDateTimeRangeGroupSettings-Eigenschaft. Gibt das Interne der Gruppe zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/
---
## PivotDateTimeRangeGroupSettings.Interval property

Ruft das Interne der Gruppe ab.

```csharp
public double Interval { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotDateTimeRangeGroupSettingsPropertyIntervalDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Fügen Sie ein Arbeitsblatt mit Beispieldaten hinzu
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Beispieldatumdaten hinzufügen
            dataSheet.Cells["A1"].PutValue("Date");
            dataSheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-5));
            dataSheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-4));
            dataSheet.Cells["A4"].PutValue(DateTime.Now.AddDays(-3));
            dataSheet.Cells["A5"].PutValue(DateTime.Now.AddDays(-2));
            dataSheet.Cells["A6"].PutValue(DateTime.Now.AddDays(-1));
            dataSheet.Cells["A7"].PutValue(DateTime.Now);

            // Ein Pivot-Tabellen-Arbeitsblatt hinzufügen
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            
            // PivotTable hinzufügen
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:A7", 
                "A1", 
                "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Füge das Datumsfeld zum Zeilenbereich hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            PivotField dateField = pivotTable.RowFields[0];

            // Nach Tagen gruppieren mit einem Intervall von 2
            dateField.GroupBy(1, false);
            PivotDateTimeRangeGroupSettings groupSettings = 
                (PivotDateTimeRangeGroupSettings)dateField.GroupSettings;
            
            // Da Interval schreibgeschützt ist, müssen wir es während der Gruppierung festlegen
            // Das Intervall wird tatsächlich in den Parametern der GroupBy-Methode festgelegt
            // Hier überprüfen wir nur den Intervallwert
            Console.WriteLine($"Grouping interval: {groupSettings.Interval} days");

            // Speichere die Arbeitsmappe
            workbook.Save("PivotDateTimeGroupingDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


