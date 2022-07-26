---
title: WorksheetCollection
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in en samling avWorksheet./worksheet objekt.
type: docs
weight: 6520
url: /sv/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Kapslar in en samling av[`Worksheet`](../worksheet) objekt.

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex) { get; set; } | Representerar indexet för aktivt kalkylblad när kalkylarket öppnas. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname) { get; set; } | Representerar namnet på det aktiva kalkylbladet när kalkylarket öppnas. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties) { get; } | Returnerar en[`DocumentProperty`](../../aspose.cells.properties/documentproperty)samling som representerar alla inbyggda dokumentegenskaper i kalkylarket. |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties) { get; } | Returnerar en[`DocumentProperty`](../../aspose.cells.properties/documentproperty) samling som representerar alla anpassade dokumentegenskaper i kalkylarket. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs) { get; } | Hämtar master differentialformateringsposter. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks) { get; } | Representerar externa länkar i en arbetsbok. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections) { get; set; } | Indikerar om alla anslutningar uppdateras när filen öppnas i MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item) { get; } | Får[`Worksheet`](../worksheet) element vid angivet index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names) { get; } | Hämtar samlingen av alla Name-objekt i kalkylarket. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize) { get; set; } | Hämtar och ställer in den visade storleken när arbetsboksfilen används som ett Ole-objekt. |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs) { get; } | Representerar revisionsloggar. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles) { get; } | Blir[`TableStyles`](./tablestyles) objekt. |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors) { get; } | Hämtar listan över trådade kommentarsförfattare. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions) { get; } | Hämtar listan över aktivitetsrutor. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes) { get; } | Hämtar listan över aktivitetsrutor. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps) { get; set; } | Hämtar och ställer in XML-kartorna i arbetsboken. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add#add_1)() | Lägger till ett kalkylblad till samlingen. |
| [Add](../../aspose.cells/worksheetcollection/add#add_2)(SheetType) | Lägger till ett kalkylblad till samlingen. |
| [Add](../../aspose.cells/worksheetcollection/add#add)(string) | Lägger till ett kalkylblad till samlingen. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy)(int) | Lägger till ett kalkylblad till samlingen och kopierar data från ett existerande kalkylblad. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy_1)(string) | Lägger till ett kalkylblad till samlingen och kopierar data från ett existerande kalkylblad. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear#clear)() | Rensa alla kalkylblad. (2 methods) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables)() | Rensar pivottabeller från kalkylarket. |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange)(string, int) | Skapar en[`Range`](../range) objekt från en adress i området. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange)(string, int) | Skapar en[`Range`](../range) objekt från en adress i området. |
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
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges)() | Hämtar alla fördefinierade namngivna intervall i kalkylarket. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables)() | Hämtar alla fördefinierade namngivna intervall i kalkylarket. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname)(string) | Hämtar Range-objekt med fördefinierat namn. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname_1)(string, int, bool) | Blir[`Range`](../range) genom fördefinierat namn eller tabellens namn |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename)(string) | Hämtar kalkylbladet med kodnamnet. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert)(int, SheetType) | Infoga ett kalkylblad. |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert_1)(int, SheetType, string) | Infoga ett kalkylblad. |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int, int) |  |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables)() | Uppdaterar alla pivottabeller i WorksheetCollection. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction_1)(int, string) | Lägger till tilläggsfunktion i arbetsboken |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction)(string, string, bool) | Lägger till tilläggsfunktion i arbetsboken |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat)(int) | Tar bort elementet vid ett angivet index. (2 methods) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat_2)(string) | Tar bort elementet vid ett angivet namn. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize)(int, int, int, int) | Ställer in visad storlek när arbetsboksfil används som ett Ole-objekt. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames)() | Sorterar de definierade namnen. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet)(int, int) | Byter de två arken. |

### Exempel

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

//Lägg till ett kalkylblad
sheets.Add();

//Ändra namnet på ett kalkylblad
sheets[0].Name = "First Sheet";

//Ställ in det aktiva bladet till det andra kalkylbladet
sheets.ActiveSheetIndex = 1;

	
[Visual Basic]

Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'Lägg till ett kalkylblad
sheets.Add()

'Ändra namnet på ett kalkylblad
sheets(0).Name = "First Sheet"

'Ställ in det aktiva bladet till det andra kalkylbladet
sheets.ActiveSheetIndex = 1
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Worksheet](../worksheet)
* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
