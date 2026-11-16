---
title: "SqlScriptSaveOptions Klasse"
linktitle: "SqlScriptSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "SqlScriptSaveOptions Klasse. Kapselt das Objekt, das sqlscriptsaveoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/sqlscriptsaveoptions/
---

## SqlScriptSaveOptions class

Stellt die Optionen zum Speichern von SQL dar.

```go

type SqlScriptSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewSqlScriptSaveOptions](./newsqlscriptsaveoptions/) | Erstellt Optionen zum Speichern einer SQL-Datei. |
| [NewSqlScriptSaveOptions_SaveOptions](./newsqlscriptsaveoptions_saveoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetCheckIfTableExists](./getcheckiftableexists/) | Prüft, ob der Tabellenname vor dem Erstellen bereits existiert. |
| [SetCheckIfTableExists](./setcheckiftableexists/) | Prüft, ob der Tabellenname vor dem Erstellen bereits existiert. |
| [GetColumnTypeMap](./getcolumntypemap/) | Ermittelt und setzt die Zuordnung von Spaltentypen für verschiedene Datenbanken. |
| [SetColumnTypeMap](./setcolumntypemap/) | Ermittelt und setzt die Zuordnung von Spaltentypen für verschiedene Datenbanken. |
| [GetCheckAllDataForColumnType](./getcheckalldataforcolumntype/) | Prüft alle Daten, um den Datentyp der Spalten zu finden. |
| [SetCheckAllDataForColumnType](./setcheckalldataforcolumntype/) | Prüft alle Daten, um den Datentyp der Spalten zu finden. |
| [GetAddBlankLineBetweenRows](./getaddblanklinebetweenrows/) | Fügt zwischen jedem Datensatz eine leere Zeile ein. |
| [SetAddBlankLineBetweenRows](./setaddblanklinebetweenrows/) | Fügt zwischen jedem Datensatz eine leere Zeile ein. |
| [GetSeparator](./getseparator/) | Ermittelt und setzt das Zeichen-Trennzeichen des SQL-Skripts. |
| [SetSeparator](./setseparator/) | Ermittelt und setzt das Zeichen-Trennzeichen des SQL-Skripts. |
| [GetOperatorType](./getoperatortype/) | Ermittelt und setzt den Operator-Typ von SQL. |
| [SetOperatorType](./setoperatortype/) | Ermittelt und setzt den Operator-Typ von SQL. |
| [GetPrimaryKey](./getprimarykey/) | Stellt dar, welche Spalte der Primärschlüssel der Datentabelle ist. |
| [SetPrimaryKey](./setprimarykey/) | Stellt dar, welche Spalte der Primärschlüssel der Datentabelle ist. |
| [GetCreateTable](./getcreatetable/) | Gibt an, ob das Exportieren von SQL zum Erstellen der Tabelle erfolgt. |
| [SetCreateTable](./setcreatetable/) | Gibt an, ob das Exportieren von SQL zum Erstellen der Tabelle erfolgt. |
| [GetIdName](./getidname/) | Ermittelt und setzt den Namen der ID-Spalte. |
| [SetIdName](./setidname/) | Ermittelt und setzt den Namen der ID-Spalte. |
| [GetStartId](./getstartid/) | Ermittelt und setzt die Start-ID. |
| [SetStartId](./setstartid/) | Ermittelt und setzt die Start-ID. |
| [GetTableName](./gettablename/) | Ermittelt und setzt den Tabellennamen. |
| [SetTableName](./settablename/) | Ermittelt und setzt den Tabellennamen. |
| [GetExportAsString](./getexportasstring/) | Gibt an, ob alle Daten als Zeichenkettenwert exportiert werden. |
| [SetExportAsString](./setexportasstring/) | Gibt an, ob alle Daten als Zeichenkettenwert exportiert werden. |
| [GetSheetIndexes](./getsheetindexes/) | Stellt die Indizes der exportierten Tabellenblätter dar. |
| [SetSheetIndexes](./setsheetindexes/) | Stellt die Indizes der exportierten Tabellenblätter dar. |
| [GetExportArea](./getexportarea/) | Liest oder setzt den Exportbereich. |
| [SetExportArea](./setexportarea/) | Liest oder setzt den Exportbereich. |
| [GetHasHeaderRow](./gethasheaderrow/) | Gibt an, ob der Bereich eine Kopfzeile enthält. |
| [SetHasHeaderRow](./sethasheaderrow/) | Gibt an, ob der Bereich eine Kopfzeile enthält. |
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
