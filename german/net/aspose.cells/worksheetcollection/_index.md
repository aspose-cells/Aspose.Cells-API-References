---
title: WorksheetCollection
second_title: Aspose.Cells für .NET-API-Referenz
description: Kapselt eine Sammlung vonWorksheet./worksheet Objekte.
type: docs
weight: 6520
url: /de/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Kapselt eine Sammlung von[`Worksheet`](../worksheet) Objekte.

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex) { get; set; } | Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname) { get; set; } | Repräsentiert den Namen des aktiven Arbeitsblatts, wenn die Tabelle geöffnet wird. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties) { get; } | Gibt a zurück[`DocumentProperty`](../../aspose.cells.properties/documentproperty)Sammlung, die alle integrierten Dokumenteigenschaften der Tabelle darstellt. |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties) { get; } | Gibt a zurück[`DocumentProperty`](../../aspose.cells.properties/documentproperty) Sammlung, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs) { get; } | Ruft die differenziellen Master-Formatierungsdatensätze ab. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks) { get; } | Repräsentiert externe Links in einer Arbeitsmappe. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections) { get; set; } | Gibt an, ob alle Verbindungen beim Öffnen einer Datei in MS Excel aktualisiert werden. |
| [Item](../../aspose.cells/worksheetcollection/item) { get; } | Ruft die ab[`Worksheet`](../worksheet) Element am angegebenen Index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names) { get; } | Ruft die Sammlung aller Name-Objekte in der Tabelle ab. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize) { get; set; } | Ruft die angezeigte Größe ab und legt sie fest, wenn die Arbeitsmappendatei als Ole-Objekt verwendet wird. |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs) { get; } | Stellt Revisionsprotokolle dar. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles) { get; } | erhält[`TableStyles`](./tablestyles) Objekt. |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors) { get; } | Ruft die Liste der Thread-Kommentarautoren ab. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions) { get; } | Ruft die Liste der Aufgabenbereiche ab. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes) { get; } | Ruft die Liste der Aufgabenbereiche ab. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps) { get; set; } | Ruft die XML-Zuordnungen in der Arbeitsmappe ab und legt sie fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add#add_1)() | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [Add](../../aspose.cells/worksheetcollection/add#add_2)(SheetType) | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [Add](../../aspose.cells/worksheetcollection/add#add)(string) | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy)(int) | Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten aus einem vorhandenen Arbeitsblatt. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy_1)(string) | Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten aus einem vorhandenen Arbeitsblatt. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear#clear)() | Alle Arbeitsblätter löschen. (2 methods) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables)() | Löscht Pivot-Tabellen aus der Tabelle. |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange)(string, int) | Erstellt ein[`Range`](../range) Objekt aus einer Adresse des Bereichs. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange)(string, int) | Erstellt ein[`Range`](../range) Objekt aus einer Adresse des Bereichs. |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges)() | Ruft alle vordefinierten benannten Bereiche in der Tabelle ab. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables)() | Ruft alle vordefinierten benannten Bereiche in der Tabelle ab. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname)(string) | Ruft Range-Objekt nach vordefiniertem Namen ab. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname_1)(string, int, bool) | erhält[`Range`](../range) nach vordefiniertem Namen oder Tabellenname |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename)(string) | Ruft das Arbeitsblatt nach dem Codenamen ab. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert)(int, SheetType) | Arbeitsblatt einfügen. |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert_1)(int, SheetType, string) | Arbeitsblatt einfügen. |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int, int) |  |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables)() | Aktualisiert alle PivotTables in der WorksheetCollection. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction_1)(int, string) | Fügt der Arbeitsmappe eine Add-in-Funktion hinzu |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction)(string, string, bool) | Fügt der Arbeitsmappe eine Add-in-Funktion hinzu |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat)(int) | Entfernt das Element an einem angegebenen Index. (2 methods) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat_2)(string) | Entfernt das Element unter einem angegebenen Namen. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize)(int, int, int, int) | Legt die angezeigte Größe fest, wenn die Arbeitsmappendatei als Ole-Objekt verwendet wird. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames)() | Sortiert die definierten Namen. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet)(int, int) | Vertauscht die beiden Blätter. |

### Beispiele

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

//Arbeitsblatt hinzufügen
sheets.Add();

//Ändern Sie den Namen eines Arbeitsblatts
sheets[0].Name = "First Sheet";

//Das aktive Blatt auf das zweite Arbeitsblatt setzen
sheets.ActiveSheetIndex = 1;

	
[Visual Basic]

Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'Fügen Sie ein Arbeitsblatt hinzu
sheets.Add()

'Ändern Sie den Namen eines Arbeitsblatts
sheets(0).Name = "First Sheet"

'Legen Sie das aktive Blatt auf das zweite Arbeitsblatt fest
sheets.ActiveSheetIndex = 1
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Worksheet](../worksheet)
* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
