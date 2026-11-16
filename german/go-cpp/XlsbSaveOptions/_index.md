---
title: "XlsbSaveOptions-Klasse"
linktitle: "XlsbSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "XlsbSaveOptions-Klasse. Kapselt das Objekt, das xlsbsaveoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/xlsbsaveoptions/
---

## XlsbSaveOptions class

Stellt die Optionen zum Speichern einer xlsb‑Datei dar.

```go

type XlsbSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewXlsbSaveOptions](./newxlsbsaveoptions/) | Erstellt Speicheroptionen für xlsb-Dateien. |
| [NewXlsbSaveOptions_SaveOptions](./newxlsbsaveoptions_saveoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetCompressionType](./getcompressiontype/) | Liest und setzt den Kompressionstyp für ooxml-Dateien. |
| [SetCompressionType](./setcompressiontype/) | Liest und setzt den Kompressionstyp für ooxml-Dateien. |
| [GetExportAllColumnIndexes](./getexportallcolumnindexes/) | Gibt an, ob alle Spaltenindizes für Zellen exportiert werden. |
| [SetExportAllColumnIndexes](./setexportallcolumnindexes/) | Gibt an, ob alle Spaltenindizes für Zellen exportiert werden. |
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
