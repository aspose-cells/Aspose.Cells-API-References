---
title: "Klasse PivotFieldGroupOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Pivot.PivotFieldGroupOptions Klasse. Optionen für die Gruppierungseinstellungen von Pivot-Feldern"
type: docs
url: /de/net/aspose.cells.pivot/pivotfieldgroupoptions/
---
## PivotFieldGroupOptions class

Optionen für die Gruppierungseinstellungen des Pivot-Felds.

```csharp
public class PivotFieldGroupOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PivotFieldGroupOptions](pivotfieldgroupoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DiscreteGroupItems](../../aspose.cells.pivot/pivotfieldgroupoptions/discretegroupitems/) { get; set; } | Liest und setzt diskrete Gruppenelemente. |
| [EndDate](../../aspose.cells.pivot/pivotfieldgroupoptions/enddate/) { get; set; } | Liest oder setzt den Endwert des Gruppierungsbereichs. |
| [EndNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/endnumber/) { get; set; } | Liest oder setzt den Endwert des Gruppierungsbereichs. |
| [GroupType](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptype/) { get; set; } | Liest oder setzt den Gruppierungstyp für das Pivot‑Feld. Nur für die Gruppierung von Datum‑Uhrzeit‑Pivot‑Feldern. |
| [GroupTypes](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptypes/) { get; set; } | Liest oder setzt den Gruppierungstyp für das Pivot‑Feld. |
| [Interval](../../aspose.cells.pivot/pivotfieldgroupoptions/interval/) { get; set; } | Liest oder setzt die Intervallgröße für jede Gruppe. |
| [IsAutoEnd](../../aspose.cells.pivot/pivotfieldgroupoptions/isautoend/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Endwert automatisch bestimmt wird. |
| [IsAutoStart](../../aspose.cells.pivot/pivotfieldgroupoptions/isautostart/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Startwert automatisch bestimmt wird. |
| [NewPivotField](../../aspose.cells.pivot/pivotfieldgroupoptions/newpivotfield/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob nach dem Gruppieren neue Pivot‑Felder erstellt werden sollen. |
| [StartDate](../../aspose.cells.pivot/pivotfieldgroupoptions/startdate/) { get; set; } | Liest oder setzt den Startwert des Gruppierungsbereichs. |
| [StartNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/startnumber/) { get; set; } | Liest oder setzt den Startwert des Gruppierungsbereichs. |

### Beispiele

```csharp

[C#]

// Lade die Beispielarbeitsmappe
Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
// Greife auf das zweite Arbeitsblatt und seine Pivot‑Tabelle zu
PivotTable pt = wb.Worksheets[1].PivotTables[0];
// Gruppiere das erste Zeilenfeld (ein Datumsfeld) nach Monaten und Quartalen
PivotFieldGroupOptions options = new PivotFieldGroupOptions();
options.StartDate = new DateTime(2008, 1, 1);
options.EndDate = new DateTime(2008, 9, 5);
options.GroupTypes = new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Quarters };
pt.RowFields[0].Group(options);
// Berechne die Pivot‑Tabellendaten und speichere die Ausgabedatei
pt.CalculateData();
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx");

[Visual Basic]

'Load the sample workbook
Dim wb As New Workbook("sampleGroupPivotFieldsInPivotTable.xlsx")
'Access the second worksheet and its pivot table
Dim pt As PivotTable = wb.Worksheets(1).PivotTables(0)
'Group the first row field (a date field) by months and quarters
Dim options As New PivotFieldGroupOptions()
options.StartDate = New DateTime(2008, 1, 1)
options.EndDate = New DateTime(2008, 9, 5)
options.GroupTypes = New PivotGroupByType() {PivotGroupByType.Months, PivotGroupByType.Quarters}
pt.RowFields(0).Group(options)
'Calculate the pivot table data and save the output file
pt.CalculateData()
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx")
```

### Siehe auch

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


