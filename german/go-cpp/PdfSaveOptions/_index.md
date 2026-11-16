---
title: "PdfSaveOptions Klasse"
linktitle: "PdfSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PdfSaveOptions-Klasse. Kapselt das Objekt, das pdfsaveoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pdfsaveoptions/
---

## PdfSaveOptions class

Stellt die Optionen zum Speichern einer PDF‑Datei dar.

```go

type PdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewPdfSaveOptions](./newpdfsaveoptions/) | Erstellt die Optionen zum Speichern einer PDF-Datei. |
| [NewPdfSaveOptions_PaginatedSaveOptions](./newpdfsaveoptions_paginatedsaveoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetEmbedStandardWindowsFonts](./getembedstandardwindowsfonts/) | True, um TrueType-Schriften einzubetten. Betrifft nur ASCII-Zeichen 32‑127. Schriften für Zeichenkodierungen größer als 127 werden immer eingebettet. Schriften werden für den PDF/A‑1a‑ und PDF/A‑1b‑Standard immer eingebettet. Standard ist true. |
| [SetEmbedStandardWindowsFonts](./setembedstandardwindowsfonts/) | True, um TrueType-Schriften einzubetten. Betrifft nur ASCII-Zeichen 32‑127. Schriften für Zeichenkodierungen größer als 127 werden immer eingebettet. Schriften werden für den PDF/A‑1a‑ und PDF/A‑1b‑Standard immer eingebettet. Standard ist true. |
| [GetBookmark](./getbookmark/) | Liest und setzt das PdfBookmarkEntry</see>-Objekt. |
| [SetBookmark](./setbookmark/) | Liest und setzt das PdfBookmarkEntry</see>-Objekt. |
| [GetCompliance](./getcompliance/) | Liest oder setzt das Konformitätsniveau der PDF-Standards für Ausgabedokumente. |
| [SetCompliance](./setcompliance/) | Liest oder setzt das Konformitätsniveau der PDF-Standards für Ausgabedokumente. |
| [GetSecurityOptions](./getsecurityoptions/) | Setzen Sie diese Optionen, wenn Sicherheit im xls2pdf-Ergebnis benötigt wird. |
| [SetSecurityOptions](./setsecurityoptions/) | Setzen Sie diese Optionen, wenn Sicherheit im xls2pdf-Ergebnis benötigt wird. |
| [GetCalculateFormula](./getcalculateformula/) | Gibt an, ob Formeln vor dem Speichern der PDF-Datei berechnet werden sollen. |
| [SetCalculateFormula](./setcalculateformula/) | Gibt an, ob Formeln vor dem Speichern der PDF-Datei berechnet werden sollen. |
| [GetPdfCompression](./getpdfcompression/) | Gibt den Komprimierungsalgorithmus an |
| [SetPdfCompression](./setpdfcompression/) | Gibt den Komprimierungsalgorithmus an |
| [SetImageResample](./setimageresample/) | Legt die gewünschte PPI (Pixel pro Zoll) für das Resampeln von Bildern und die JPEG-Qualität fest. Alle Bilder werden mit der angegebenen Qualitätseinstellung in JPEG konvertiert, und Bilder, die größer als die angegebene PPI (Pixel pro Zoll) sind, werden resampelt. |
| [GetCreatedTime](./getcreatedtime/) | Liest und setzt die Erstellungszeit des PDF-Dokuments. |
| [SetCreatedTime](./setcreatedtime/) | Liest und setzt die Erstellungszeit des PDF-Dokuments. |
| [GetProducer](./getproducer/) | Liest und setzt den Ersteller des erzeugten PDF-Dokuments. |
| [SetProducer](./setproducer/) | Liest und setzt den Ersteller des erzeugten PDF-Dokuments. |
| [GetOptimizationType](./getoptimizationtype/) | Liest und setzt den PDF-Optimierungstyp. |
| [SetOptimizationType](./setoptimizationtype/) | Liest und setzt den PDF-Optimierungstyp. |
| [GetCustomPropertiesExport](./getcustompropertiesexport/) | Liest oder setzt einen Wert, der bestimmt, wie CustomDocumentPropertyCollection in eine PDF-Datei exportiert werden. Standardwert ist None. |
| [SetCustomPropertiesExport](./setcustompropertiesexport/) | Liest oder setzt einen Wert, der bestimmt, wie CustomDocumentPropertyCollection in eine PDF-Datei exportiert werden. Standardwert ist None. |
| [GetExportDocumentStructure](./getexportdocumentstructure/) | Gibt an, ob die Dokumentstruktur exportiert werden soll. |
| [SetExportDocumentStructure](./setexportdocumentstructure/) | Gibt an, ob die Dokumentstruktur exportiert werden soll. |
| [GetDisplayDocTitle](./getdisplaydoctitle/) | Gibt an, ob die Titelleiste des Fensters den Dokumenttitel anzeigen soll. |
| [SetDisplayDocTitle](./setdisplaydoctitle/) | Gibt an, ob die Titelleiste des Fensters den Dokumenttitel anzeigen soll. |
| [GetFontEncoding](./getfontencoding/) | Liest oder setzt die eingebettete Schriftkodierung im PDF. |
| [SetFontEncoding](./setfontencoding/) | Liest oder setzt die eingebettete Schriftkodierung im PDF. |
| [GetWatermark](./getwatermark/) | Liest oder setzt das Wasserzeichen für die Ausgabe. |
| [SetWatermark](./setwatermark/) | Liest oder setzt das Wasserzeichen für die Ausgabe. |
| [GetEmbedAttachments](./getembedattachments/) | Gibt an, ob Anhänge für OLE-Objekte in Excel eingebettet werden sollen. |
| [SetEmbedAttachments](./setembedattachments/) | Gibt an, ob Anhänge für OLE-Objekte in Excel eingebettet werden sollen. |
| [GetZoomBehavior](./getzoombehavior/) | Liest oder setzt den anfänglichen Ansichtsmodus, wenn das erzeugte PDF-Dokument geöffnet wird. Der Standardwert ist PdfZoomBehavior.None. |
| [SetZoomBehavior](./setzoombehavior/) | Liest oder setzt den anfänglichen Ansichtsmodus, wenn das erzeugte PDF-Dokument geöffnet wird. Der Standardwert ist PdfZoomBehavior.None. |
| [GetZoomFactor](./getzoomfactor/) | Liest oder setzt den Zoom-Prozentsatz, der verwendet wird, wenn ZoomBehavior PdfZoomBehavior.ZoomFactor ist. |
| [SetZoomFactor](./setzoomfactor/) | Liest oder setzt den Zoom-Prozentsatz, der verwendet wird, wenn ZoomBehavior PdfZoomBehavior.ZoomFactor ist. |
| [GetDefaultFont](./getdefaultfont/) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie in PDF/Bild als Block erscheinen. Setzen Sie die DefaultFont, z. B. MingLiu oder MS Gothic, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft nicht festgelegt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode-Zeichen anzuzeigen. |
| [SetDefaultFont](./setdefaultfont/) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie in PDF/Bild als Block erscheinen. Setzen Sie die DefaultFont, z. B. MingLiu oder MS Gothic, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft nicht festgelegt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode-Zeichen anzuzeigen. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie in PDF/Bild als Block erscheinen. Setzen Sie dies auf true, um zunächst zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen anzuzeigen. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie in PDF/Bild als Block erscheinen. Setzen Sie dies auf true, um zunächst zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen anzuzeigen. |
| [SetCheckFontCompatibility](./setcheckfontcompatibility/) | Gibt an, ob die Schriftartkompatibilität für jedes Zeichen im Text überprüft werden soll. |
| [GetCheckFontCompatibility](./getcheckfontcompatibility/) | Gibt an, ob die Schriftartkompatibilität für jedes Zeichen im Text überprüft werden soll. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Gibt an, ob die Schriftart eines Zeichens nur ersetzt werden soll, wenn die Zellen-Schriftart nicht kompatibel ist. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Gibt an, ob die Schriftart eines Zeichens nur ersetzt werden soll, wenn die Zellen-Schriftart nicht kompatibel ist. |
| [GetOnePagePerSheet](./getonepagepersheet/) | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blattes nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße der Seiten-einstellung wird ungültig sein, während die anderen Einstellungen der Seiten-einstellung weiterhin wirksam bleiben. |
| [SetOnePagePerSheet](./setonepagepersheet/) | Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blattes nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße der Seiten-einstellung wird ungültig sein, während die anderen Einstellungen der Seiten-einstellung weiterhin wirksam bleiben. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blattes nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße der Seiten-einstellung wird ignoriert, während die anderen Einstellungen der Seiten-einstellung weiterhin wirksam bleiben. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | Wenn AllColumnsInOnePagePerSheet true ist, wird der gesamte Spalteninhalt eines Blattes nur auf einer Seite im Ergebnis ausgegeben. Die Breite der Papiergröße der Seiten-einstellung wird ignoriert, während die anderen Einstellungen der Seiten-einstellung weiterhin wirksam bleiben. |
| [GetIgnoreError](./getignoreerror/) | Gibt an, ob Fehler beim Rendern ausgeblendet werden sollen. Der Fehler kann ein Fehler bei Formen, Bildern, Diagrammen usw. sein. |
| [SetIgnoreError](./setignoreerror/) | Gibt an, ob Fehler beim Rendern ausgeblendet werden sollen. Der Fehler kann ein Fehler bei Formen, Bildern, Diagrammen usw. sein. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist. |
| [SetPageIndex](./setpageindex/) | Liest oder setzt den nullbasierten Index der ersten zu speichernden Seite. |
| [GetPageIndex](./getpageindex/) | Liest oder setzt den nullbasierten Index der ersten zu speichernden Seite. |
| [SetPageCount](./setpagecount/) | Liest oder setzt die Anzahl der zu speichernden Seiten. |
| [GetPageCount](./getpagecount/) | Liest oder setzt die Anzahl der zu speichernden Seiten. |
| [GetPrintingPageType](./getprintingpagetype/) | Gibt an, welche Seiten nicht gedruckt werden. |
| [SetPrintingPageType](./setprintingpagetype/) | Gibt an, welche Seiten nicht gedruckt werden. |
| [GetGridlineType](./getgridlinetype/) | Liest oder setzt den Rasterlinientyp. |
| [SetGridlineType](./setgridlinetype/) | Liest oder setzt den Rasterlinientyp. |
| [GetGridlineColor](./getgridlinecolor/) | Liest oder setzt die Rasterlinienfarbe. |
| [SetGridlineColor](./setgridlinecolor/) | Liest oder setzt die Rasterlinienfarbe. |
| [GetTextCrossType](./gettextcrosstype/) | Liest oder legt den Anzeigetexttyp fest, wenn die Textbreite größer als die Zellenbreite ist. |
| [SetTextCrossType](./settextcrosstype/) | Liest oder legt den Anzeigetexttyp fest, wenn die Textbreite größer als die Zellenbreite ist. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | Liest oder legt die Standardsprache für die Bearbeitung fest. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | Liest oder legt die Standardsprache für die Bearbeitung fest. |
| [GetSheetSet](./getsheetset/) | Liest oder legt die zu rendernden Arbeitsblätter fest. Standard ist: Alle sichtbaren Arbeitsblätter in der Arbeitsmappe: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Liest oder legt die zu rendernden Arbeitsblätter fest. Standard ist: Alle sichtbaren Arbeitsblätter in der Arbeitsmappe: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Implementiert dieses Interface, um DrawObject und Bound beim Rendern zu erhalten. |
| [GetEmfRenderSetting](./getemfrendersetting/) | Einstellung für das Rendern von EMF-Metadateien. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Einstellung für das Rendern von EMF-Metadateien. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Liest oder legt benutzerdefinierte Einstellungen während des Renderns fest. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Liest oder legt benutzerdefinierte Einstellungen während des Renderns fest. |
| [GetRenderingBehavior](./getrenderingbehavior/) | Liest oder legt die anzuwendenden Excel-spezifischen Rendering‑Verhalten fest. |
| [SetRenderingBehavior](./setrenderingbehavior/) | Liest oder legt die anzuwendenden Excel-spezifischen Rendering‑Verhalten fest. |
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
