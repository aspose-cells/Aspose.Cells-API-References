---
title: "MarkdownSaveOptions-Klasse"
linktitle: "MarkdownSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "MarkdownSaveOptions-Klasse. Kapselt das Objekt, das markdownsaveoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

Stellt die Speicheroptionen für Markdown dar.

```go

type MarkdownSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewMarkdownSaveOptions](./newmarkdownsaveoptions/) | Erstellt Optionen zum Speichern eines Markdown-Dokuments |
| [NewMarkdownSaveOptions_SaveOptions](./newmarkdownsaveoptions_saveoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetEncoding](./getencoding/) | Liest und setzt die Standardkodierung. |
| [SetEncoding](./setencoding/) | Liest und setzt die Standardkodierung. |
| [GetFormatStrategy](./getformatstrategy/) | Liest und setzt die Formatierungsstrategie beim Exportieren des Zellenwerts als Zeichenkette. |
| [SetFormatStrategy](./setformatstrategy/) | Liest und setzt die Formatierungsstrategie beim Exportieren des Zellenwerts als Zeichenkette. |
| [GetLineSeparator](./getlineseparator/) | Liest und setzt den Zeilentrenner. |
| [SetLineSeparator](./setlineseparator/) | Liest und setzt den Zeilentrenner. |
| [GetTableHeaderType](./gettableheadertype/) | Liest und legt fest, wie der Tabellenkopf gesetzt wird. |
| [SetTableHeaderType](./settableheadertype/) | Liest und legt fest, wie der Tabellenkopf gesetzt wird. |
| [GetSheetSet](./getsheetset/) | Liest oder legt die zu rendernden Arbeitsblätter fest. Standard ist: alle sichtbaren Arbeitsblätter in der Arbeitsmappe: Aspose.Cells.Rendering.SheetSet.Active. |
| [SetSheetSet](./setsheetset/) | Liest oder legt die zu rendernden Arbeitsblätter fest. Standard ist: alle sichtbaren Arbeitsblätter in der Arbeitsmappe: Aspose.Cells.Rendering.SheetSet.Active. |
| [GetImageOptions](./getimageoptions/) | Rufen Sie das ImageOrPrintOptions-Objekt vor dem Exportieren ab |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | Gibt an, ob Bilder im Base64-Format in Markdown gespeichert werden. Der Standardwert ist true. |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | Gibt an, ob Bilder im Base64-Format in Markdown gespeichert werden. Der Standardwert ist true. |
| [GetCalculateFormula](./getcalculateformula/) | Gibt an, ob Formeln vor dem Speichern der Markdown-Datei berechnet werden sollen. |
| [SetCalculateFormula](./setcalculateformula/) | Gibt an, ob Formeln vor dem Speichern der Markdown-Datei berechnet werden sollen. |
| [GetExportHyperlinkAsReference](./getexporthyperlinkasreference/) | Gibt an, ob Hyperlinks mittels Referenzdefinitionen anstelle des Inline-Formats exportiert werden sollen. Der Standardwert ist false. |
| [SetExportHyperlinkAsReference](./setexporthyperlinkasreference/) | Gibt an, ob Hyperlinks mittels Referenzdefinitionen anstelle des Inline-Formats exportiert werden sollen. Der Standardwert ist false. |
| [GetAlignColumnPadding](./getaligncolumnpadding/) | Gibt an, ob die Spaltenausrichtung für erzeugte Markdown-Tabellen aktiviert ist. Wenn aktiviert, werden Spalten durch Auffüllen des Zelleninhalts mit dem angegebenen Zeichen (typischerweise ' ' für Leerzeichen) ausgerichtet. Setze auf '\\0', um die Spaltenausrichtung zu deaktivieren (Standard). |
| [SetAlignColumnPadding](./setaligncolumnpadding/) | Gibt an, ob die Spaltenausrichtung für erzeugte Markdown-Tabellen aktiviert ist. Wenn aktiviert, werden Spalten durch Auffüllen des Zelleninhalts mit dem angegebenen Zeichen (typischerweise ' ' für Leerzeichen) ausgerichtet. Setze auf '\\0', um die Spaltenausrichtung zu deaktivieren (Standard). |
| [GetSplitTablesByBlankRow](./getsplittablesbyblankrow/) | Gibt an, ob leere Zeilen im Arbeitsblatt beim Export nach Markdown als Tabellentrenner behandelt werden sollen. Der Standardwert ist false. |
| [SetSplitTablesByBlankRow](./setsplittablesbyblankrow/) | Gibt an, ob leere Zeilen im Arbeitsblatt beim Export nach Markdown als Tabellentrenner behandelt werden sollen. Der Standardwert ist false. |
| [GetOfficeMathOutputType](./getofficemathoutputtype/) | Gibt an, wie OfficeMath-Objekte nach Markdown exportiert werden. Der Standardwert ist Bild. |
| [SetOfficeMathOutputType](./setofficemathoutputtype/) | Gibt an, wie OfficeMath-Objekte nach Markdown exportiert werden. Der Standardwert ist Bild. |
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
