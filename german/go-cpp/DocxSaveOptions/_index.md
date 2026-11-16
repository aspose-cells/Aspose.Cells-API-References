---
title: "DocxSaveOptions Klasse"
linktitle: "DocxSaveOptions"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "DocxSaveOptions-Klasse. Kapselt das Objekt, das docxsaveoptions in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/docxsaveoptions/
---

## DocxSaveOptions class

Stellt die Optionen zum Speichern einer .docx‑Datei dar.

```go

type DocxSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewDocxSaveOptions](./newdocxsaveoptions/) | Stellt die Optionen zum Speichern einer .docx‑Datei dar. |
| [NewDocxSaveOptions_Bool](./newdocxsaveoptions_bool/) | Stellt die Optionen zum Speichern einer .docx‑Datei dar. |
| [NewDocxSaveOptions_PaginatedSaveOptions](./newdocxsaveoptions_paginatedsaveoptions/) | Konstruiert aus einem übergeordneten Objekt. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetSaveAsEditableShapes](./getsaveaseditableshapes/) | Speichern Sie alle Zeichenobjekte als editierbare Formen in der Word-Datei, sodass Sie sie in Word bearbeiten können. |
| [SetSaveAsEditableShapes](./setsaveaseditableshapes/) | Speichern Sie alle Zeichenobjekte als editierbare Formen in der Word-Datei, sodass Sie sie in Word bearbeiten können. |
| [GetEmbedXlsxAsChartDataSource](./getembedxlsxaschartdatasource/) | Gibt an, ob eine xlsx-Datei als Datenquelle des Diagramms eingebettet wird. |
| [SetEmbedXlsxAsChartDataSource](./setembedxlsxaschartdatasource/) | Gibt an, ob eine xlsx-Datei als Datenquelle des Diagramms eingebettet wird. |
| [GetAsFlatOpc](./getasflatopc/) | Gibt an, ob als flache OPC-Datei gespeichert wird, die vom Open XML SDK erzeugt werden kann. |
| [SetAsFlatOpc](./setasflatopc/) | Gibt an, ob als flache OPC-Datei gespeichert wird, die vom Open XML SDK erzeugt werden kann. |
| [GetSaveElementType](./getsaveelementtype/) | Gibt an, welche Elemente gespeichert werden sollen. |
| [SetSaveElementType](./setsaveelementtype/) | Gibt an, welche Elemente gespeichert werden sollen. |
| [GetAsNormalView](./getasnormalview/) | Exportieren der Excel-Datei nach docx-Datei in der Normalansicht. Wenn diese Eigenschaft true ist, wird ein Bereich ausgegeben, und keine Skalierung wird wirksam. Der Standardwert ist false. |
| [SetAsNormalView](./setasnormalview/) | Exportieren der Excel-Datei nach docx-Datei in der Normalansicht. Wenn diese Eigenschaft true ist, wird ein Bereich ausgegeben, und keine Skalierung wird wirksam. Der Standardwert ist false. |
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
