---
title: "JsonSaveOptions-Klasse"
linktitle: "JsonSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "JsonSaveOptions-Klasse. Kapselt das Objekt, das jsonsaveoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/jsonsaveoptions/
---

## JsonSaveOptions class

Stellt die Optionen zum Speichern der Arbeitsmappe als JSON-Datei dar.

```go

type JsonSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewJsonSaveOptions](./newjsonsaveoptions/) | Erstellt Optionen zum Speichern einer JSON-Datei. |
| [NewJsonSaveOptions_SaveOptions](./newjsonsaveoptions_saveoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetExportStylePool](./getexportstylepool/) | Gibt an, ob Stile gesammelt oder einzeln in jede Zelle exportiert werden sollen. |
| [SetExportStylePool](./setexportstylepool/) | Gibt an, ob Stile gesammelt oder einzeln in jede Zelle exportiert werden sollen. |
| [GetExportHyperlinkType](./getexporthyperlinktype/) | Stellt den Typ des Exports von Hyperlinks nach JSON dar. |
| [SetExportHyperlinkType](./setexporthyperlinktype/) | Stellt den Typ des Exports von Hyperlinks nach JSON dar. |
| [GetSkipEmptyRows](./getskipemptyrows/) | Gibt an, ob leere Zeilen übersprungen werden. |
| [SetSkipEmptyRows](./setskipemptyrows/) | Gibt an, ob leere Zeilen übersprungen werden. |
| [GetSheetIndexes](./getsheetindexes/) | Stellt die Indizes der exportierten Tabellenblätter dar. |
| [SetSheetIndexes](./setsheetindexes/) | Stellt die Indizes der exportierten Tabellenblätter dar. |
| [GetSchemas](./getschemas/) | Das ursprüngliche JSON-Schema jedes Arbeitsblatts. |
| [SetSchemas](./setschemas/) | Das ursprüngliche JSON-Schema jedes Arbeitsblatts. |
| [GetExportArea](./getexportarea/) | Liest oder setzt den Exportbereich. |
| [SetExportArea](./setexportarea/) | Liest oder setzt den Exportbereich. |
| [GetHasHeaderRow](./gethasheaderrow/) | Gibt an, ob der Bereich eine Kopfzeile enthält. |
| [SetHasHeaderRow](./sethasheaderrow/) | Gibt an, ob der Bereich eine Kopfzeile enthält. |
| [GetExportAsString](./getexportasstring/) | Exportiert den Zeichenkettenwert der Zellen nach JSON. |
| [SetExportAsString](./setexportasstring/) | Exportiert den Zeichenkettenwert der Zellen nach JSON. |
| [GetIndent](./getindent/) | Gibt die Einrückung an. |
| [SetIndent](./setindent/) | Gibt die Einrückung an. |
| [GetExportNestedStructure](./getexportnestedstructure/) | Exportiert als übergeordnete/untergeordnete hierarchische JSON-Struktur. |
| [SetExportNestedStructure](./setexportnestedstructure/) | Exportiert als übergeordnete/untergeordnete hierarchische JSON-Struktur. |
| [GetExportEmptyCells](./getexportemptycells/) | Gibt an, ob leere Zellen als null exportiert werden. |
| [SetExportEmptyCells](./setexportemptycells/) | Gibt an, ob leere Zellen als null exportiert werden. |
| [GetAlwaysExportAsJsonObject](./getalwaysexportasjsonobject/) | Gibt an, ob Excel immer als Objekt nach JSON exportiert wird, selbst wenn die Datei nur ein Arbeitsblatt enthält. |
| [SetAlwaysExportAsJsonObject](./setalwaysexportasjsonobject/) | Gibt an, ob Excel immer als Objekt nach JSON exportiert wird, selbst wenn die Datei nur ein Arbeitsblatt enthält. |
| [GetToExcelStruct](./gettoexcelstruct/) | Gibt an, ob in die JSON-Struktur der Excel-Datei konvertiert wird. |
| [SetToExcelStruct](./settoexcelstruct/) | Gibt an, ob in die JSON-Struktur der Excel-Datei konvertiert wird. |
| [GetSaveFormat](./getsaveformat/) | Ermittelt das Dateiformat zum Speichern. |
| [GetClearData](./getcleardata/) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [SetClearData](./setcleardata/) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [GetCachedFileFolder](./getcachedfilefolder/) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [SetCachedFileFolder](./setcachedfilefolder/) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden sollen. |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden sollen. |
| [GetMergeAreas](./getmergeareas/) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden sollen. |
| [SetMergeAreas](./setmergeareas/) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden sollen. |
| [GetCreateDirectory](./getcreatedirectory/) | Wenn wahr und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [SetCreateDirectory](./setcreatedirectory/) | Wenn wahr und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [GetSortNames](./getsortnames/) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden sollen. |
| [SetSortNames](./setsortnames/) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden sollen. |
| [GetSortExternalNames](./getsortexternalnames/) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden sollen. |
| [SetSortExternalNames](./setsortexternalnames/) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden sollen. |
| [GetRefreshChartCache](./getrefreshchartcache/) | Gibt an, ob die neuesten Daten des Diagramms zwischengespeichert werden sollen. |
| [SetRefreshChartCache](./setrefreshchartcache/) | Gibt an, ob die neuesten Daten des Diagramms zwischengespeichert werden sollen. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Ob Beschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB eingeben, wird er abgeschnitten. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Ob Beschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB eingeben, wird er abgeschnitten. |
| [GetUpdateSmartArt](./getupdatesmartart/) | Gibt an, ob die SmartArt-Einstellung aktualisiert wird. Der Standardwert ist false. |
| [SetUpdateSmartArt](./setupdatesmartart/) | Gibt an, ob die SmartArt-Einstellung aktualisiert wird. Der Standardwert ist false. |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true. |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true. |
