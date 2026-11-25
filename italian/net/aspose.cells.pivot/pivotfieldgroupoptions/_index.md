---
title: "Classe PivotFieldGroupOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Pivot.PivotFieldGroupOptions. Opzioni per le impostazioni di raggruppamento del campo pivot"
type: docs
url: /it/net/aspose.cells.pivot/pivotfieldgroupoptions/
---
## PivotFieldGroupOptions class

Opzioni per le impostazioni di raggruppamento del campo pivot.

```csharp
public class PivotFieldGroupOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PivotFieldGroupOptions](pivotfieldgroupoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DiscreteGroupItems](../../aspose.cells.pivot/pivotfieldgroupoptions/discretegroupitems/) { get; set; } | Ottiene e imposta gli elementi di gruppo discreti. |
| [EndDate](../../aspose.cells.pivot/pivotfieldgroupoptions/enddate/) { get; set; } | Ottiene o imposta il valore finale dell'intervallo di raggruppamento. |
| [EndNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/endnumber/) { get; set; } | Ottiene o imposta il valore finale dell'intervallo di raggruppamento. |
| [GroupType](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptype/) { get; set; } | Ottiene o imposta il tipo di raggruppamento per il campo pivot. Solo per il raggruppamento del campo pivot data e ora. |
| [GroupTypes](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptypes/) { get; set; } | Ottiene o imposta il tipo di raggruppamento per il campo pivot. |
| [Interval](../../aspose.cells.pivot/pivotfieldgroupoptions/interval/) { get; set; } | Ottiene o imposta la dimensione dell'intervallo per ogni gruppo. |
| [IsAutoEnd](../../aspose.cells.pivot/pivotfieldgroupoptions/isautoend/) { get; set; } | Ottiene o imposta un valore che indica se il valore finale è determinato automaticamente. |
| [IsAutoStart](../../aspose.cells.pivot/pivotfieldgroupoptions/isautostart/) { get; set; } | Ottiene o imposta un valore che indica se il valore iniziale è determinato automaticamente. |
| [NewPivotField](../../aspose.cells.pivot/pivotfieldgroupoptions/newpivotfield/) { get; set; } | Ottiene o imposta un valore che indica se nuovi campi pivot devono essere creati dopo il raggruppamento. |
| [StartDate](../../aspose.cells.pivot/pivotfieldgroupoptions/startdate/) { get; set; } | Ottiene o imposta il valore iniziale dell'intervallo di raggruppamento. |
| [StartNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/startnumber/) { get; set; } | Ottiene o imposta il valore iniziale dell'intervallo di raggruppamento. |

### Esempi

```csharp

[C#]

// Carica la cartella di lavoro di esempio
Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
// Accedi al secondo foglio di lavoro e alla sua tabella pivot
PivotTable pt = wb.Worksheets[1].PivotTables[0];
// Raggruppa il primo campo di riga (un campo data) per mesi e trimestri
PivotFieldGroupOptions options = new PivotFieldGroupOptions();
options.StartDate = new DateTime(2008, 1, 1);
options.EndDate = new DateTime(2008, 9, 5);
options.GroupTypes = new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Quarters };
pt.RowFields[0].Group(options);
// Calcola i dati della tabella pivot e salva il file di output
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

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


