---
title: "Klass PivotFieldGroupOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotFieldGroupOptions-klass. Alternativ för inställningar för gruppering av pivottfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldgroupoptions/
---
## PivotFieldGroupOptions class

Alternativ för inställningar för gruppering av pivottfält.

```csharp
public class PivotFieldGroupOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PivotFieldGroupOptions](pivotfieldgroupoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DiscreteGroupItems](../../aspose.cells.pivot/pivotfieldgroupoptions/discretegroupitems/) { get; set; } | Hämtar och anger diskreta grupperingselement. |
| [EndDate](../../aspose.cells.pivot/pivotfieldgroupoptions/enddate/) { get; set; } | Hämtar eller anger slutvärdet för grupperingens intervall. |
| [EndNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/endnumber/) { get; set; } | Hämtar eller anger slutvärdet för grupperingens intervall. |
| [GroupType](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptype/) { get; set; } | Hämtar eller anger grupperingstypen för pivottfält. Endast för gruppering av datum‑tid‑pivottfält. |
| [GroupTypes](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptypes/) { get; set; } | Hämtar eller anger grupperingstypen för pivottfält. |
| [Interval](../../aspose.cells.pivot/pivotfieldgroupoptions/interval/) { get; set; } | Hämtar eller anger intervallstorleken för varje grupp. |
| [IsAutoEnd](../../aspose.cells.pivot/pivotfieldgroupoptions/isautoend/) { get; set; } | Hämtar eller anger ett värde som indikerar om slutvärdet bestäms automatiskt. |
| [IsAutoStart](../../aspose.cells.pivot/pivotfieldgroupoptions/isautostart/) { get; set; } | Hämtar eller anger ett värde som indikerar om startvärdet bestäms automatiskt. |
| [NewPivotField](../../aspose.cells.pivot/pivotfieldgroupoptions/newpivotfield/) { get; set; } | Hämtar eller anger ett värde som indikerar om nya pivottfält ska skapas efter gruppering. |
| [StartDate](../../aspose.cells.pivot/pivotfieldgroupoptions/startdate/) { get; set; } | Hämtar eller anger startvärdet för grupperingens intervall. |
| [StartNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/startnumber/) { get; set; } | Hämtar eller anger startvärdet för grupperingens intervall. |

### Exempel

```csharp

[C#]

// Läs in exempelarbetsboken
Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
// Få åtkomst till det andra kalkylbladet och dess pivottabell
PivotTable pt = wb.Worksheets[1].PivotTables[0];
// Gruppera det första radfältet (ett datumfält) efter månader och kvartal
PivotFieldGroupOptions options = new PivotFieldGroupOptions();
options.StartDate = new DateTime(2008, 1, 1);
options.EndDate = new DateTime(2008, 9, 5);
options.GroupTypes = new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Quarters };
pt.RowFields[0].Group(options);
// Beräkna pivottabelldata och spara utdatafilen
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

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


