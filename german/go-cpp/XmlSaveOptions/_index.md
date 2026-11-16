---
title: "XmlSaveOptions Klasse"
linktitle: "XmlSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "XmlSaveOptions Klasse. Kapselt das Objekt, das xmlsaveoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/xmlsaveoptions/
---

## XmlSaveOptions class

Stellt die Optionen zum Speichern der Arbeitsmappe als XML‑Datei dar.

```go

type XmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewXmlSaveOptions](./newxmlsaveoptions/) | Erstellt Optionen zum Speichern einer XML-Datei. |
| [NewXmlSaveOptions_SaveOptions](./newxmlsaveoptions_saveoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetSheetIndexes](./getsheetindexes/) | Stellt die Indizes der exportierten Tabellenblätter dar. |
| [SetSheetIndexes](./setsheetindexes/) | Stellt die Indizes der exportierten Tabellenblätter dar. |
| [GetExportArea](./getexportarea/) | Liest oder setzt den Exportbereich. |
| [SetExportArea](./setexportarea/) | Liest oder setzt den Exportbereich. |
| [GetHasHeaderRow](./gethasheaderrow/) | Gibt an, ob der Bereich eine Kopfzeile enthält. |
| [SetHasHeaderRow](./sethasheaderrow/) | Gibt an, ob der Bereich eine Kopfzeile enthält. |
| [GetXmlMapName](./getxmlmapname/) | Gibt an, ob eine XML-Karte in der Datei exportiert wird. |
| [SetXmlMapName](./setxmlmapname/) | Gibt an, ob eine XML-Karte in der Datei exportiert wird. |
| [GetSheetNameAsElementName](./getsheetnameaselementname/) | Gibt an, ob der Blattname als Name des Elements exportiert wird. |
| [SetSheetNameAsElementName](./setsheetnameaselementname/) | Gibt an, ob der Blattname als Name des Elements exportiert wird. |
| [GetDataAsAttribute](./getdataasattribute/) | Gibt an, ob Daten als Attribute des Elements exportiert werden. |
| [SetDataAsAttribute](./setdataasattribute/) | Gibt an, ob Daten als Attribute des Elements exportiert werden. |
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
