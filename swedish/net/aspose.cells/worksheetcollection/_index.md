---
title: "Klass WorksheetCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.WorksheetCollection-klass. Inkapslar en samling av Worksheet-objekt"
type: docs
url: /sv/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Inkapslar en samling av [`Worksheet`](../worksheet/) objekt.

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex/) { get; set; } | Representerar indexet för det aktiva kalkylbladet när kalkylarket öppnas. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname/) { get; set; } | Representerar namnet på det aktiva kalkylbladet när kalkylarket öppnas. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties/) { get; } | Returnerar en [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) samling som representerar alla inbyggda dokumentegenskaper i kalkylarket. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties/) { get; } | Returnerar en [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) samling som representerar alla anpassade dokumentegenskaper i kalkylarket. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs/) { get; } | Hämtar huvudposterna för differentialformatering. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks/) { get; } | Representerar externa länkar i en arbetsbok. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections/) { get; set; } | Anger om alla anslutningar ska uppdateras vid öppning av filen i MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item/) { get; } | Hämtar [`Worksheet`](../worksheet/) elementet på det angivna indexet. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names/) { get; } | Hämtar samlingen av alla Name-objekt i kalkylarket. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize/) { get; set; } | Hämtar och anger visad storlek när Workbook-filen används som ett Ole-objekt. |
| [PivotCaches](../../aspose.cells/worksheetcollection/pivotcaches/) { get; } | Hämtar alla [`PivotCache`](../../aspose.cells.pivot/pivotcache/). |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs/) { get; } | Representerar revisionsloggar. |
| [SensitivityLabels](../../aspose.cells/worksheetcollection/sensitivitylabels/) { get; } | Representerar alla känslighetsetiketter. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles/) { get; } | Hämtar [`TableStyles`](./tablestyles/) objekt. |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors/) { get; } | Hämtar listan över författare till trådade kommentarer. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions/) { get; } | Hämtar listan över uppgiftspaneler. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes/) { get; } | Hämtar listan över uppgiftspaneler. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps/) { get; set; } | Hämtar och anger XML-kartor i arbetsboken. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add/#add_1)() | Lägger till ett kalkylblad i samlingen. |
| [Add](../../aspose.cells/worksheetcollection/add/#add_2)(SheetType) | Lägger till ett kalkylblad i samlingen. |
| [Add](../../aspose.cells/worksheetcollection/add/#add)(string) | Lägger till ett kalkylblad i samlingen. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy)(int) | Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_1)(string) | Lägger till ett kalkylblad i samlingen och kopierar data från ett befintligt kalkylblad. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_2)(Worksheet[], string[]) | Kopiera en grupp kalkylblad. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear/#clear)() | Rensa alla kalkylblad. (2 metoder) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables/)() | Rensar pivottabeller från kalkylbladet. |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange/)(string, int) | Skapar ett [`Range`](../range/)‑objekt från en adress för området. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange/)(string, int) | Skapar ett [`Range`](../range/)‑objekt från en adress för området. |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges/)() | Hämtar alla fördefinierade namngivna områden i kalkylbladet. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables/)() | Hämtar alla fördefinierade namngivna områden i kalkylbladet. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname)(string) | Hämtar Range‑objektet efter fördefinierat namn. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname_1)(string, int, bool) | Hämtar [`Range`](../range/) efter fördefinierat namn eller tabellens namn |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename/)(string) | Hämtar kalkylbladet efter kodnamnet. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert)(int, SheetType) | Infoga ett kalkylblad. |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert_1)(int, SheetType, string) | Infoga ett kalkylblad. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int, int) |  |
| [RefreshAll](../../aspose.cells/worksheetcollection/refreshall/)() | (**Föråldrad.**) Uppdatera alla pivottabeller och diagram med pivottkällan. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables_1)() | Uppdaterar alla PivotTables i Excel‑filen. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables)(PivotTableRefreshOption) | Uppdaterar alla PivotTables i Excel‑filen. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction_1)(int, string) | Lägger till tilläggsfunktion i arbetsboken |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction)(string, string, bool) | Lägger till tilläggsfunktion i arbetsboken |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat)(int) | Tar bort elementet på ett angivet index. (2 metoder) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat_2)(string) | Tar bort elementet med ett angivet namn. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize/)(int, int, int, int) | Ställer in visad storlek när Workbook‑filen används som ett Ole‑objekt. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames/)() | Sorterar de definierade namnen. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet/)(int, int) | Byter plats på de två bladen. |

### Exempel

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionDemo
    {
        public static void RunDemo()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;

            // Lägg till ett nytt kalkylblad i samlingen
            int newSheetIndex = worksheets.Add(SheetType.Worksheet);
            Worksheet newSheet = worksheets[newSheetIndex];
            newSheet.Name = "NewSheet";

            // Åtkomst till ett befintligt kalkylblad via index
            Worksheet firstSheet = worksheets[0];
            firstSheet.Name = "FirstSheet";

            // Åtkomst till ett befintligt kalkylblad via namn
            Worksheet retrievedSheet = worksheets["FirstSheet"];

            // Ställ in det aktiva bladet
            worksheets.ActiveSheetIndex = newSheetIndex;

            // Ställ in det aktiva bladets namn
            worksheets.ActiveSheetName = "NewSheet";

            // Uppdatera alla pivottabeller i arbetsboken
            worksheets.RefreshAll();

            // Rensa alla pivottabeller från arbetsboken
            worksheets.ClearPivottables();

            // Spara arbetsboken
            workbook.Save("WorksheetCollectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Worksheet](../worksheet/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


