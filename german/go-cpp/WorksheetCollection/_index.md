---
title: "WorksheetCollection Klasse"
linktitle: "WorksheetCollection"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "WorksheetCollection Klasse. Kapselt das Objekt, das worksheetcollection in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/worksheetcollection/
---

## WorksheetCollection class

Kapselt eine Sammlung von <see cref=\"Worksheet\"/> Objekten.

```go

type WorksheetCollection struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetWebExtensionTaskPanes](./getwebextensiontaskpanes/) | Liest die Liste der Aufgabenbereiche. |
| [GetWebExtensions](./getwebextensions/) | Liest die Liste der Aufgabenbereiche. |
| [GetThreadedCommentAuthors](./getthreadedcommentauthors/) | Liest die Liste der Autoren von Threaded-Kommentaren. |
| [IsRefreshAllConnections](./isrefreshallconnections/) | Gibt an, ob beim Öffnen einer Datei in MS Excel alle Verbindungen aktualisiert werden. |
| [SetIsRefreshAllConnections](./setisrefreshallconnections/) | Gibt an, ob beim Öffnen einer Datei in MS Excel alle Verbindungen aktualisiert werden. |
| [CreateRange](./createrange/) | Erstellt ein Range-Objekt aus einer Adresse des Bereichs. |
| [CreateUnionRange](./createunionrange/) | Erstellt ein Range-Objekt aus einer Adresse des Bereichs. |
| [GetNames](./getnames/) | Liest die Sammlung aller Namensobjekte im Tabellenblatt. |
| [Get_Int](./get_int/) | Liefert das Worksheet-Element am angegebenen Index. |
| [Get_String](./get_string/) | Liefert das Worksheet-Element mit dem angegebenen Namen. |
| [GetSheetByCodeName](./getsheetbycodename/) | Liefert das Worksheet über den Codenamen. |
| [GetActiveSheetName](./getactivesheetname/) | Stellt den Namen des aktiven Worksheets dar, wenn die Tabelle geöffnet wird. |
| [SetActiveSheetName](./setactivesheetname/) | Stellt den Namen des aktiven Worksheets dar, wenn die Tabelle geöffnet wird. |
| [GetActiveSheetIndex](./getactivesheetindex/) | Stellt den Index des aktiven Worksheets dar, wenn die Tabelle geöffnet wird. |
| [SetActiveSheetIndex](./setactivesheetindex/) | Stellt den Index des aktiven Worksheets dar, wenn die Tabelle geöffnet wird. |
| [SortNames](./sortnames/) | Sortiert die definierten Namen. |
| [Insert_Int_SheetType](./insert_int_sheettype/) | Fügt ein Worksheet ein. |
| [Insert_Int_SheetType_String](./insert_int_sheettype_string/) | Fügt ein Worksheet ein. |
| [Add_SheetType](./add_sheettype/) | Fügt ein Worksheet zur Sammlung hinzu. |
| [SwapSheet](./swapsheet/) | Vertauscht die beiden Blätter. |
| [Add](./add/) | Fügt ein Worksheet zur Sammlung hinzu. |
| [Add_String](./add_string/) | Fügt ein Worksheet zur Sammlung hinzu. |
| [RegisterAddInFunction_String_String_Bool](./registeraddinfunction_string_string_bool/) | Fügt eine Add-In-Funktion in die Arbeitsmappe ein. |
| [RegisterAddInFunction_Int_String](./registeraddinfunction_int_string/) | Fügt eine Add-In-Funktion in die Arbeitsmappe ein. |
| [RemoveAt_String](./removeat_string/) | Entfernt das Element mit einem angegebenen Namen. |
| [RemoveAt_Int](./removeat_int/) | Entfernt das Element an einem angegebenen Index. |
| [Clear](./clear/) | Alle Worksheets löschen. |
| [AddCopy_String](./addcopy_string/) | Fügt ein Worksheet zur Sammlung hinzu und kopiert Daten von einem bestehenden Worksheet. |
| [AddCopy_Int](./addcopy_int/) | Fügt ein Worksheet zur Sammlung hinzu und kopiert Daten von einem bestehenden Worksheet. |
| [AddCopy_WorksheetArray_stringArray](./addcopy_worksheetarray_stringarray/) | Kopiere eine Gruppe von Worksheets. |
| [GetDxfs](./getdxfs/) | Liefert die Master-Differenzformatierungsdatensätze. |
| [GetRangeByName_String](./getrangebyname_string/) | Liefert das Range-Objekt über einen vordefinierten Namen. |
| [GetRangeByName_String_Int_Bool](./getrangebyname_string_int_bool/) | Liefert das Range über einen vordefinierten Namen oder den Tabellennamen |
| [GetNamedRanges](./getnamedranges/) | Liefert alle vordefinierten benannten Bereiche in der Tabelle. |
| [GetNamedRangesAndTables](./getnamedrangesandtables/) | Liefert alle vordefinierten benannten Bereiche in der Tabelle. |
| [GetXmlMaps](./getxmlmaps/) | Liefert und setzt die XML-Maps in der Arbeitsmappe. |
| [SetXmlMaps](./setxmlmaps/) | Liefert und setzt die XML-Maps in der Arbeitsmappe. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Gibt eine DocumentProperty‑Sammlung zurück, die alle integrierten Dokumenteigenschaften der Tabelle darstellt. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Gibt eine DocumentProperty‑Sammlung zurück, die alle benutzerdefinierten Dokumenteigenschaften der Tabelle darstellt. |
| [GetOleSize](./getolesize/) | Liefert und setzt die angezeigte Größe, wenn die Arbeitsmappe als OLE-Objekt verwendet wird. |
| [SetOleSize_Object](./setolesize_object/) | Liefert und setzt die angezeigte Größe, wenn die Arbeitsmappe als OLE-Objekt verwendet wird. |
| [SetOleSize_Int_Int_Int_Int](./setolesize_int_int_int_int/) | Setzt die angezeigte Größe, wenn die Arbeitsmappe als OLE-Objekt verwendet wird. |
| [GetExternalLinks](./getexternallinks/) | Stellt externe Links in einer Arbeitsmappe dar. |
| [GetPivotCaches](./getpivotcaches/) | Liefert alle PivotCache. |
| [GetTableStyles](./gettablestyles/) | Liefert das TableStyles-Objekt. |
| [ClearPivottables](./clearpivottables/) | Löscht Pivot-Tabellen aus der Kalkulationstabelle. |
| [GetRevisionLogs](./getrevisionlogs/) | Stellt Revisionsprotokolle dar. |
| [RefreshPivotTables](./refreshpivottables/) | Aktualisiert alle PivotTables in der Excel-Datei. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Aktualisiert alle PivotTables in der Excel-Datei. |
| [GetSensitivityLabels](./getsensitivitylabels/) | Stellt alle Sensitivitätskennzeichnungen dar. |
| [GetCount](./getcount/) | Liefert die Anzahl der im Objekt enthaltenen Elemente. |
