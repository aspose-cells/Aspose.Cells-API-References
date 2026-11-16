---
title: "TxtSaveOptions Class"
linktitle: "TxtSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "TxtSaveOptions class. Kapselt das Objekt, das die TxtSaveOptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/txtsaveoptions/
---

## TxtSaveOptions class

Stellt die Speicheroptionen für CSV/Tab-getrenntes/anderes Textformat dar.

```go

type TxtSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewTxtSaveOptions](./newtxtsaveoptions/) | Erstellt Optionen zum Speichern von Textdateien. |
| [NewTxtSaveOptions_SaveFormat](./newtxtsaveoptions_saveformat/) | Erstellt Optionen zum Speichern von Textdateien. |
| [NewTxtSaveOptions_SaveOptions](./newtxtsaveoptions_saveoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetSeparator](./getseparator/) | Liest und setzt das Zeichen-Trennzeichen der Textdatei. |
| [SetSeparator](./setseparator/) | Liest und setzt das Zeichen-Trennzeichen der Textdatei. |
| [GetSeparatorString](./getseparatorstring/) | Liest und setzt einen Zeichenkettenwert als Trennzeichen. |
| [SetSeparatorString](./setseparatorstring/) | Liest und setzt einen Zeichenkettenwert als Trennzeichen. |
| [GetEncoding](./getencoding/) | Liest und setzt die Standardkodierung. |
| [SetEncoding](./setencoding/) | Liest und setzt die Standardkodierung. |
| [GetQuoteType](./getquotetype/) | Liest oder setzt, wie Werte in der exportierten Textdatei zitiert werden. |
| [SetQuoteType](./setquotetype/) | Liest oder setzt, wie Werte in der exportierten Textdatei zitiert werden. |
| [GetFormatStrategy](./getformatstrategy/) | Liest und setzt die Formatierungsstrategie beim Exportieren des Zellenwerts als Zeichenkette. |
| [SetFormatStrategy](./setformatstrategy/) | Liest und setzt die Formatierungsstrategie beim Exportieren des Zellenwerts als Zeichenkette. |
| [GetTrimLeadingBlankRowAndColumn](./gettrimleadingblankrowandcolumn/) | Gibt an, ob führende leere Zeilen und Spalten wie in MS Excel entfernt werden sollen. Standard ist true. |
| [SetTrimLeadingBlankRowAndColumn](./settrimleadingblankrowandcolumn/) | Gibt an, ob führende leere Zeilen und Spalten wie in MS Excel entfernt werden sollen. Standard ist true. |
| [GetTrimTailingBlankCells](./gettrimtailingblankcells/) | Gibt an, ob nachfolgende leere Zellen in einer Zeile entfernt werden sollen. Standard ist false. |
| [SetTrimTailingBlankCells](./settrimtailingblankcells/) | Gibt an, ob nachfolgende leere Zellen in einer Zeile entfernt werden sollen. Standard ist false. |
| [GetKeepSeparatorsForBlankRow](./getkeepseparatorsforblankrow/) | Gibt an, ob Trennzeichen für leere Zeilen ausgegeben werden sollen. Der Standardwert ist false, sodass der Inhalt für leere Zeilen standardmäßig leer ist. |
| [SetKeepSeparatorsForBlankRow](./setkeepseparatorsforblankrow/) | Gibt an, ob Trennzeichen für leere Zeilen ausgegeben werden sollen. Der Standardwert ist false, sodass der Inhalt für leere Zeilen standardmäßig leer ist. |
| [GetExportArea](./getexportarea/) | Der Bereich der zu exportierenden Zellen. |
| [SetExportArea](./setexportarea/) | Der Bereich der zu exportierenden Zellen. |
| [GetExportQuotePrefix](./getexportquoteprefix/) | Gibt an, ob das einfache Anführungszeichen als Teil des Werts einer Zelle exportiert werden soll, wenn Style.QuotePrefix für diese Zelle true ist. Standard ist false. |
| [SetExportQuotePrefix](./setexportquoteprefix/) | Gibt an, ob das einfache Anführungszeichen als Teil des Werts einer Zelle exportiert werden soll, wenn Style.QuotePrefix für diese Zelle true ist. Standard ist false. |
| [GetExportAllSheets](./getexportallsheets/) | Gibt an, ob alle Arbeitsblätter in die Textdatei exportiert werden sollen. Ist es false, wird nur das aktive Arbeitsblatt exportiert, ähnlich wie bei MS Excel. |
| [SetExportAllSheets](./setexportallsheets/) | Gibt an, ob alle Arbeitsblätter in die Textdatei exportiert werden sollen. Ist es false, wird nur das aktive Arbeitsblatt exportiert, ähnlich wie bei MS Excel. |
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
