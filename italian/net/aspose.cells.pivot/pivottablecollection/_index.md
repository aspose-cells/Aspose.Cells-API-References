---
title: PivotTableCollection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta la raccolta di tutti gli oggetti tabella pivot nel foglio di lavoro specificato.
type: docs
weight: 4710
url: /it/net/aspose.cells.pivot/pivottablecollection/
---
## PivotTableCollection class

Rappresenta la raccolta di tutti gli oggetti tabella pivot nel foglio di lavoro specificato.

```csharp
public class PivotTableCollection : CollectionBase<PivotTable>, IDisposable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.pivot/pivottablecollection/item) { get; } | Ottiene il rapporto della tabella pivot per indice. (3 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_1)(PivotTable, string, string) | Aggiunge un nuovo oggetto tabella pivot alla raccolta da un'altra tabella pivot. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_4)(string, string, string) | Aggiunge una nuova cache di tabella pivot a una raccolta di PivotCaches. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add)(PivotTable, int, int, string) | Aggiunge un nuovo oggetto tabella pivot alla raccolta da un'altra tabella pivot. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_2)(string, int, int, string) | Aggiunge una nuova cache di tabella pivot a una raccolta di PivotCaches. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_5)(string, string, string, bool) | Aggiunge una nuova cache di tabella pivot a una raccolta di PivotCaches. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_3)(string, int, int, string, bool) | Aggiunge una nuova cache di tabella pivot a una raccolta di PivotCaches. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_7)(string[], bool, PivotPageFields, string, string) | Aggiunge un nuovo oggetto tabella pivot alla raccolta con più intervalli di consolidamento come origine dati. |
| [Add](../../aspose.cells.pivot/pivottablecollection/add#add_6)(string[], bool, PivotPageFields, int, int, string) | Aggiunge un nuovo oggetto tabella pivot alla raccolta con più intervalli di consolidamento come origine dati. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(PivotTable) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(PivotTable, IComparer&lt;PivotTable&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, PivotTable, IComparer&lt;PivotTable&gt;) |  |
| [Clear](../../aspose.cells.pivot/pivottablecollection/clear#clear)() | Cancella tutte le tabelle pivot. (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(PivotTable) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(PivotTable[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(PivotTable[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, PivotTable[], int, int) |  |
| [Dispose](../../aspose.cells.pivot/pivottablecollection/dispose)() | Esegue attività definite dall'applicazione associate alla liberazione, rilascio o ripristino di risorse non gestite. |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;PivotTable&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;PivotTable&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;PivotTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;PivotTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;PivotTable&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;PivotTable&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;PivotTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;PivotTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;PivotTable&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;PivotTable&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(PivotTable) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(PivotTable, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(PivotTable, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(PivotTable) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(PivotTable, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(PivotTable, int, int) |  |
| [Remove](../../aspose.cells.pivot/pivottablecollection/remove#remove)(PivotTable) | Elimina la tabella pivot specificata ed elimina i dati della tabella pivot |
| [Remove](../../aspose.cells.pivot/pivottablecollection/remove#remove_1)(PivotTable, bool) | Elimina la tabella pivot specificata |
| [RemoveAt](../../aspose.cells.pivot/pivottablecollection/removeat#removeat)(int) | Elimina la tabella pivot in corrispondenza dell'indice specificato ed elimina i dati della tabella pivot (2 methods) |
| [RemoveAt](../../aspose.cells.pivot/pivottablecollection/removeat#removeat_2)(int, bool) | Elimina la tabella pivot in corrispondenza dell'indice specificato |

### Esempi

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

//Modifica gli attributi di PivotField
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//Aggiungi filtro pivot
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

//Aggiungi PivotFormatCondition
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

//fai i tuoi affari

book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'Aggiungi filtro pivot
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'Aggiungi PivotFormatCondition
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Guarda anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [PivotTable](../pivottable)
* spazio dei nomi [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
