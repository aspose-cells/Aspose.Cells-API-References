---
title: "Klasse WorksheetCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WorksheetCollection Klasse. Kapselt eine Sammlung von Worksheet‑Objekten."
type: docs
url: /de/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Kapselt eine Sammlung von [`Worksheet`](../worksheet/) Objekten.

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex/) { get; set; } | Stellt den Index des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname/) { get; set; } | Stellt den Namen des aktiven Arbeitsblatts dar, wenn die Tabelle geöffnet wird. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties/) { get; } | Gibt eine [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) Sammlung zurück, die alle integrierten Dokumenteigenschaften der Tabelle darstellt. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties/) { get; } | Gibt eine [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs/) { get; } | Ruft die Master-Differenzformatierungsdatensätze ab. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks/) { get; } | Stellt externe Links in einer Arbeitsmappe dar. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections/) { get; set; } | Gibt an, ob beim Öffnen der Datei in MS Excel alle Verbindungen aktualisiert werden. |
| [Item](../../aspose.cells/worksheetcollection/item/) { get; } | Ruft das [`Worksheet`](../worksheet/)‑Element am angegebenen Index ab. (2 Indexer) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names/) { get; } | Ruft die Sammlung aller Name‑Objekte im Tabellenblatt ab. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize/) { get; set; } | Ruft die angezeigte Größe ab und legt sie fest, wenn die Arbeitsmappendatei als Ole‑Objekt verwendet wird. |
| [PivotCaches](../../aspose.cells/worksheetcollection/pivotcaches/) { get; } | Ruft alle [`PivotCache`](../../aspose.cells.pivot/pivotcache/) ab. |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs/) { get; } | Stellt Revisionsprotokolle dar. |
| [SensitivityLabels](../../aspose.cells/worksheetcollection/sensitivitylabels/) { get; } | Stellt alle Sensitivitätskennzeichnungen dar. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles/) { get; } | Ruft das [`TableStyles`](./tablestyles/)‑Objekt ab. |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors/) { get; } | Ruft die Liste der Autoren von Thread‑Kommentaren ab. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions/) { get; } | Ruft die Liste der Aufgabenbereiche ab. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes/) { get; } | Ruft die Liste der Aufgabenbereiche ab. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps/) { get; set; } | Ruft die XML‑Karten in der Arbeitsmappe ab und legt sie fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add/#add_1)() | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [Add](../../aspose.cells/worksheetcollection/add/#add_2)(SheetType) | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [Add](../../aspose.cells/worksheetcollection/add/#add)(string) | Fügt der Sammlung ein Arbeitsblatt hinzu. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy)(int) | Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_1)(string) | Fügt der Sammlung ein Arbeitsblatt hinzu und kopiert Daten von einem bestehenden Arbeitsblatt. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_2)(Worksheet[], string[]) | Kopiert eine Gruppe von Arbeitsblättern. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear/#clear)() | Löscht alle Arbeitsblätter. (2 Methoden) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables/)() | Löscht Pivot‑Tabellen aus dem Tabellenblatt. |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange/)(string, int) | Erstellt ein [`Range`](../range/)‑Objekt aus einer Adresse des Bereichs. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange/)(string, int) | Erstellt ein [`Range`](../range/)‑Objekt aus einer Adresse des Bereichs. |
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
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges/)() | Ruft alle vordefinierten benannten Bereiche im Tabellenblatt ab. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables/)() | Ruft alle vordefinierten benannten Bereiche im Tabellenblatt ab. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname)(string) | Ruft das Range‑Objekt über einen vordefinierten Namen ab. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname_1)(string, int, bool) | Ruft [`Range`](../range/) über einen vordefinierten Namen oder den Tabellennamen ab |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename/)(string) | Ruft das Arbeitsblatt über den Codenamen ab. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert)(int, SheetType) | Fügt ein Arbeitsblatt ein. |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert_1)(int, SheetType, string) | Fügt ein Arbeitsblatt ein. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int, int) |  |
| [RefreshAll](../../aspose.cells/worksheetcollection/refreshall/)() | (**Obsolete.**) Aktualisiert alle Pivot‑Tabellen und Diagramme mit der Pivot‑Quelle. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables_1)() | Aktualisiert alle PivotTables in der Excel-Datei. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables)(PivotTableRefreshOption) | Aktualisiert alle PivotTables in der Excel-Datei. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction_1)(int, string) | Fügt die Add‑In‑Funktion in die Arbeitsmappe ein. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction)(string, string, bool) | Fügt die Add‑In‑Funktion in die Arbeitsmappe ein. |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat)(int) | Entfernt das Element an einem angegebenen Index. (2 Methoden) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat_2)(string) | Entfernt das Element mit einem angegebenen Namen. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize/)(int, int, int, int) | Setzt die angezeigte Größe, wenn die Workbook-Datei als Ole-Objekt verwendet wird. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames/)() | Sortiert die definierten Namen. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet/)(int, int) | Vertauscht die beiden Blätter. |

### Beispiele

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionDemo
    {
        public static void RunDemo()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;

            // Fügt ein neues Arbeitsblatt zur Sammlung hinzu.
            int newSheetIndex = worksheets.Add(SheetType.Worksheet);
            Worksheet newSheet = worksheets[newSheetIndex];
            newSheet.Name = "NewSheet";

            // Greift per Index auf ein vorhandenes Arbeitsblatt zu.
            Worksheet firstSheet = worksheets[0];
            firstSheet.Name = "FirstSheet";

            // Greift per Name auf ein vorhandenes Arbeitsblatt zu.
            Worksheet retrievedSheet = worksheets["FirstSheet"];

            // Setze das aktive Blatt.
            worksheets.ActiveSheetIndex = newSheetIndex;

            // Setze den Namen des aktiven Blatts.
            worksheets.ActiveSheetName = "NewSheet";

            // Aktualisiere alle PivotTables in der Arbeitsmappe.
            worksheets.RefreshAll();

            // Lösche alle PivotTables aus der Arbeitsmappe.
            worksheets.ClearPivottables();

            // Speichere die Arbeitsmappe
            workbook.Save("WorksheetCollectionDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Worksheet](../worksheet/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


