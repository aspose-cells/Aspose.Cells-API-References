---
title: "OoxmlSaveOptions Klasse"
linktitle: "OoxmlSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "OoxmlSaveOptions Klasse. Kapselt das Objekt, das ooxmlsaveoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/ooxmlsaveoptions/
---

## OoxmlSaveOptions class

Stellt die Optionen zum Speichern einer Office Open XML‑Datei dar.

```go

type OoxmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewOoxmlSaveOptions](./newooxmlsaveoptions/) | Erstellt die Optionen zum Speichern einer Office Open XML-Datei. |
| [NewOoxmlSaveOptions_SaveFormat](./newooxmlsaveoptions_saveformat/) | Erstellt die Optionen zum Speichern einer Office Open XML-Datei. |
| [NewOoxmlSaveOptions_SaveOptions](./newooxmlsaveoptions_saveoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetAsFlatOpc](./getasflatopc/) | Gibt an, ob als flache OPC-Datei gespeichert wird, die vom Open XML SDK erzeugt werden kann. |
| [SetAsFlatOpc](./setasflatopc/) | Gibt an, ob als flache OPC-Datei gespeichert wird, die vom Open XML SDK erzeugt werden kann. |
| [GetExportCellName](./getexportcellname/) | Gibt an, ob der Zellname in Excel2007 .xlsx (.xlsm, .xltx, .xltm) Datei exportiert wird. Wenn die Ausgabedatei von SQL Server DTS verwendet werden kann, muss dieser Wert true sein. Das Setzen des Werts auf false erhöht die Leistung erheblich und reduziert die Dateigröße beim Erstellen großer Dateien. Standardwert ist true. |
| [SetExportCellName](./setexportcellname/) | Gibt an, ob der Zellname in Excel2007 .xlsx (.xlsm, .xltx, .xltm) Datei exportiert wird. Wenn die Ausgabedatei von SQL Server DTS verwendet werden kann, muss dieser Wert true sein. Das Setzen des Werts auf false erhöht die Leistung erheblich und reduziert die Dateigröße beim Erstellen großer Dateien. Standardwert ist true. |
| [GetUpdateZoom](./getupdatezoom/) | Gibt an, ob der Skalierungsfaktor vor dem Speichern der Datei aktualisiert wird, wenn die Eigenschaften PageSetup.FitToPagesWide und PageSetup.FitToPagesTall steuern, wie das Arbeitsblatt skaliert wird. |
| [SetUpdateZoom](./setupdatezoom/) | Gibt an, ob der Skalierungsfaktor vor dem Speichern der Datei aktualisiert wird, wenn die Eigenschaften PageSetup.FitToPagesWide und PageSetup.FitToPagesTall steuern, wie das Arbeitsblatt skaliert wird. |
| [GetEnableZip64](./getenablezip64/) | Verwende ZIP64-Erweiterungen beim Schreiben von ZIP-Archiven, falls erforderlich. |
| [SetEnableZip64](./setenablezip64/) | Verwende ZIP64-Erweiterungen beim Schreiben von ZIP-Archiven, falls erforderlich. |
| [GetEmbedOoxmlAsOleObject](./getembedooxmlasoleobject/) | Gibt an, ob Ooxml-Dateien von OleObject als Ole-Objekt eingebettet werden. |
| [SetEmbedOoxmlAsOleObject](./setembedooxmlasoleobject/) | Gibt an, ob Ooxml-Dateien von OleObject als Ole-Objekt eingebettet werden. |
| [GetCompressionType](./getcompressiontype/) | Liest und setzt den Kompressionstyp für ooxml-Dateien. |
| [SetCompressionType](./setcompressiontype/) | Liest und setzt den Kompressionstyp für ooxml-Dateien. |
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
