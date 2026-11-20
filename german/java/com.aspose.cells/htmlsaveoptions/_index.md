---
title: "HtmlSaveOptions"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Optionen zum Speichern einer HTML-Datei dar."
type: docs
url: /de/java/com.aspose.cells/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class HtmlSaveOptions extends SaveOptions
```

Stellt die Optionen zum Speichern einer HTML-Datei dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Erstellt Optionen zum Speichern einer HTML-Datei. |
| [HtmlSaveOptions(int saveFormat)](#HtmlSaveOptions-int-) | Erstellt Optionen zum Speichern einer HTM-Datei. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddGenericFont()](#getAddGenericFont--) | Gibt an, ob eine generische Schriftart zur CSS‑font-family hinzugefügt werden soll. |
| [getAddTooltipText()](#getAddTooltipText--) | Gibt an, ob ein Tooltip-Text hinzugefügt wird, wenn die Daten nicht vollständig angezeigt werden können. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Geben Sie das URL-Präfix für angehängte Dateien wie Bilder in der HTML-Datei an. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [getCalculateFormula()](#getCalculateFormula--) | Gibt an, ob Formeln vor dem Speichern der HTML-Datei berechnet werden sollen. |
| [getCellCssPrefix()](#getCellCssPrefix--) | Ermittelt das Präfix des CSS-Namens, der Standardwert ist "". |
| [getCellNameAttribute()](#getCellNameAttribute--) | Gibt das Attribut an, das den zu schreibenden CellName kennzeichnet. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [getCreateDirectory()](#getCreateDirectory--) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [getCssStyles()](#getCssStyles--) | Ermittelt die zusätzlichen CSS-Stile für den Formatter. |
| [getDataBarRenderMode()](#getDataBarRenderMode--) | Stellt den Modus dar, wie DataBar beim Konvertieren von Excel-Dateien in HTML-Dateien gerendert wird. |
| [getDefaultFontName()](#getDefaultFontName--) | Geben Sie den Standard-Schriftartnamen für den Export von HTML an; die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null. |
| [getDisableCss()](#getDisableCss--) | Gibt an, ob nur Inline-Stile angewendet werden, ohne sich auf CSS zu verlassen. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | Gibt an, ob Downlevel-revealed bedingte Kommentare beim Exportieren der Datei nach HTML deaktiviert werden; der Standardwert ist false. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Ermittelt den Typ der Einbettung von Schriftdateien in die HTML-Datei. |
| [getEnableCssCustomProperties()](#getEnableCssCustomProperties--) | Optimiert die HTML-Ausgabe durch die Verwendung von benutzerdefinierten CSS-Eigenschaften. |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--) | Gibt an, ob die HTML‑Zeichenentitäten durch dezimale Codes ersetzt werden. |
| [getEncoding()](#getEncoding--) | Falls nicht festgelegt, wird Encoding.UTF8 als Standard‑Kodierungstyp verwendet. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | Gibt an, ob ungenutzte Stile ausgeschlossen werden. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Gibt an, ob nur das aktive Arbeitsblatt in eine HTML‑Datei exportiert wird. |
| [getExportArea()](#getExportArea--) | Ruft den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts ab. |
| [getExportBogusRowData()](#getExportBogusRowData--) | Gibt an, ob fehlerhafte Daten der unteren Zeile exportiert werden. |
| [getExportCellCoordinate()](#getExportCellCoordinate--) | Gibt an, ob beim Speichern der Datei als HTML die Excel‑Koordinaten nicht leerer Zellen exportiert werden. |
| [getExportCommentsType()](#getExportCommentsType--) | Stellt den Typ des Exports von Kommentaren in HTML‑Dateien dar. |
| [getExportDataOptions()](#getExportDataOptions--) | Gibt die Regel für den Export von HTML‑Dateidaten an. Der Standardwert ist Alle. |
| [getExportDocumentProperties()](#getExportDocumentProperties--) | Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [getExportExtraHeadings()](#getExportExtraHeadings--) | Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger als die maximal anzeigbare Spalte ist. |
| [getExportFormula()](#getExportFormula--) | Gibt an, ob Formeln beim Speichern der Datei als HTML exportiert werden. |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--) | Gibt an, ob Frame‑Skripte und Dokumenteigenschaften exportiert werden. |
| [getExportGridLines()](#getExportGridLines--) | Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false. |
| [getExportHeadings()](#getExportHeadings--) | Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML‑Dateien exportiert werden. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Gibt an, ob der Inhalt ausgeblendeter Arbeitsblätter exportiert wird. Der Standardwert ist true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Legt fest, ob Bilder im Base64‑Format in HTML, MHTML oder EPUB gespeichert werden. |
| [getExportNamedRangeAnchors()](#getExportNamedRangeAnchors--) | Gibt an, ob Anker‑Elemente für benannte Bereiche beim Speichern als HTML exportiert werden. |
| [getExportObjectListener()](#getExportObjectListener--) | Ruft den ExportObjectListener für den Export von Objekten ab. |
| [getExportPageFooters()](#getExportPageFooters--) | Gibt an, ob Seitenkopfzeilen exportiert werden. |
| [getExportPageHeaders()](#getExportPageHeaders--) | Gibt an, ob Seitenkopfzeilen exportiert werden. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Gibt an, ob nur der Druckbereich in eine HTML‑Datei exportiert wird. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML‑Dateien exportiert werden. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | Gibt an, ob ein ähnlicher Rahmenstil exportiert wird, wenn der Rahmenstil von Browsern nicht unterstützt wird. |
| [getExportSingleTab()](#getExportSingleTab--) | Gibt an, ob das einzelne Tabellenblatt exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | Gibt an, ob Arbeitsmappeneigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | Gibt an, ob das CSS des Arbeitsblatts separat exportiert wird. Der Standardwert ist false. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | Gibt an, ob Arbeitsblatt‑Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [getFilePathProvider()](#getFilePathProvider--) | Ruft den IFilePathProvider zum separaten Exportieren des Arbeitsblatts nach HTML ab. |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--) | Gibt an, ob die vollständig formatierte Zellendaten angezeigt werden sollen, wenn die Spalte überläuft. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--) | Versteckte Spalte (die Breite dieser Spalte ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird, wenn HtmlHiddenColDisplayType auf \"Remove\" gesetzt ist, wird die versteckte Spalte nicht ausgegeben; ist der Wert \"Hidden\", wird die Spalte ausgegeben, aber verborgen. Der Standardwert ist \"Hidden\". |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--) | Versteckte Zeile (die Höhe dieser Zeile ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird, wenn HtmlHiddenRowDisplayType auf \"Remove\" gesetzt ist, wird die versteckte Zeile nicht ausgegeben; ist der Wert \"Hidden\", wird die Zeile ausgegeben, aber verborgen. Der Standardwert ist \"Hidden\". |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--) | Gibt an, ob überlaufender Text ausgeblendet werden soll, wenn das Zellenformat auf Zeilenumbruch gesetzt ist. |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--) | Gibt an, ob ein über mehrere Zellen erstreckender Text beim Speichern einer Excel‑Datei im HTML‑Format auf dieselbe Weise wie in MS Excel angezeigt wird. |
| [getHtmlVersion()](#getHtmlVersion--) | Gibt die HTML‑Standardversion an, die beim Speichern im HTML‑Format verwendet werden soll. |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--) | Gibt an, ob nicht sichtbare Formen exportiert werden. |
| [getImageOptions()](#getImageOptions--) | Rufen Sie das ImageOrPrintOptions‑Objekt vor dem Exportieren ab. |
| [getImageScalable()](#getImageScalable--) | Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird, wenn eine skalierbare Einheit zur Beschreibung der Spaltenbreite verwendet wird. |
| [getLayoutMode()](#getLayoutMode--) | Ruft den Layoutmodus beim Speichern nach HTML ab. |
| [getLinkTargetType()](#getLinkTargetType--) | Gibt den Typ des target‑Attributs im `<a>`‑Link an. |
| [getMergeAreas()](#getMergeAreas--) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--) | Gibt an, ob leere TD‑Elemente beim Exportieren der Datei nach HTML zwangsweise zusammengeführt werden. |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--) | Die Option, zusammenhängende leere Zellen (leere td‑Elemente) zusammenzuführen. Der Standardwert ist MergeEmptyTdType.Default. |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--) | Gibt an, wie OfficeMath‑Objekte nach HTML exportiert werden. Der Standardwert ist Image. |
| [getPageTitle()](#getPageTitle--) | Der Titel der HTML‑Seite. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Gibt an, ob HTML‑Tags (wie `<div></div>`) in einer Zelle als Zellwert geparst oder unverändert beibehalten werden sollen. |
| [getPresentationPreference()](#getPresentationPreference--) | Gibt an, ob HTML‑ oder MHT‑Datei die bevorzugte Darstellung ist. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen. |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--) | Gibt an, ob das HTML als einzelne Datei gespeichert werden soll. |
| [getSaveFormat()](#getSaveFormat--) | Ermittelt das Speicherdateiformat. |
| [getSheetSet()](#getSheetSet--) | Ruft die zu rendernden Arbeitsblätter ab. |
| [getShowAllSheets()](#getShowAllSheets--) | Gibt an, ob beim Speichern als einzelne HTML‑Datei alle Arbeitsblätter angezeigt werden. |
| [getSortExternalNames()](#getSortExternalNames--) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden. |
| [getSortNames()](#getSortNames--) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [getSpaceMode()](#getSpaceMode--) | Gibt an, wie Leerzeichen in der HTML‑Ausgabe gerendert werden. |
| [getStreamProvider()](#getStreamProvider--) | Ruft den IStreamProvider zum Exportieren von Objekten ab. |
| [getTableCssId()](#getTableCssId--) | Ruft das Präfix des CSS‑Typs wie tr, col, td usw. ab, das im Table‑Element enthalten ist, das das spezifische TableCssId‑Attribut besitzt. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [getWarningCallback()](#getWarningCallback--) | Liest den Warn‑Callback. |
| [getWidthScalable()](#getWidthScalable--) | Gibt an, ob die Spaltenbreite in Skalierungseinheiten nach HTML exportiert wird. |
| [getWorksheetScalable()](#getWorksheetScalable--) | Gibt an, ob beim Speichern der Datei nach HTML über das Arbeitsblatt‑Zoomlevel in das HTML hinein- oder herausgezoomt wird; der Standardwert ist false. |
| [hashCode()](#hashCode--) |  |
| [isBorderCollapsed()](#isBorderCollapsed--) | Gibt an, ob die Tabellenränder zusammengefasst sind. |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | Gibt an, ob Bilddateien in ein temporäres Verzeichnis exportiert werden. |
| [isExportComments()](#isExportComments--) | Gibt an, ob Kommentare beim Speichern der Datei nach HTML exportiert werden; der Standardwert ist false. |
| [isFullPathLink()](#isFullPathLink--) | Gibt an, ob ein vollständiger Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. |
| [isIECompatible()](#isIECompatible--) | Gibt an, ob das ausgegebene HTML mit dem IE‑Browser kompatibel ist. |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--) | Gibt an, ob JavaScript mit Browsern kompatibel ist, die kein JavaScript unterstützen. |
| [isMobileCompatible()](#isMobileCompatible--) | Gibt an, ob das ausgegebene HTML mit mobilen Geräten kompatibel ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddGenericFont(boolean value)](#setAddGenericFont-boolean-) | Gibt an, ob eine generische Schriftart zur CSS‑font-family hinzugefügt werden soll. |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | Gibt an, ob ein Tooltip-Text hinzugefügt wird, wenn die Daten nicht vollständig angezeigt werden können. |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Geben Sie das URL-Präfix für angehängte Dateien wie Bilder in der HTML-Datei an. |
| [setBorderCollapsed(boolean value)](#setBorderCollapsed-boolean-) | Gibt an, ob die Tabellenränder zusammengefasst sind. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Gibt an, ob Formeln vor dem Speichern der HTML-Datei berechnet werden sollen. |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | Legt das Präfix des CSS‑Namens fest, der Standardwert ist "". |
| [setCellNameAttribute(String value)](#setCellNameAttribute-java.lang.String-) | Gibt das Attribut an, das den zu schreibenden CellName kennzeichnet. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Ob Einschränkungen der Excel‑Datei geprüft werden, wenn der Benutzer zellenbezogene Objekte ändert. |
| [setClearData(boolean value)](#setClearData-boolean-) | Leert die Arbeitsmappe nach dem Speichern der Datei. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt. |
| [setCssStyles(String value)](#setCssStyles-java.lang.String-) | Legt die zusätzlichen CSS‑Stile für den Formatter fest. |
| [setDataBarRenderMode(int value)](#setDataBarRenderMode-int-) | Stellt den Modus dar, wie DataBar beim Konvertieren von Excel-Dateien in HTML-Dateien gerendert wird. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Geben Sie den Standard-Schriftartnamen für den Export von HTML an; die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null. |
| [setDisableCss(boolean value)](#setDisableCss-boolean-) | Gibt an, ob nur Inline-Stile angewendet werden, ohne sich auf CSS zu verlassen. |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | Gibt an, ob Downlevel-revealed bedingte Kommentare beim Exportieren der Datei nach HTML deaktiviert werden; der Standardwert ist false. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Legt den Typ des Einbettens von Schriftdateien in die HTML‑Datei fest. |
| [setEnableCssCustomProperties(boolean value)](#setEnableCssCustomProperties-boolean-) | Optimiert die HTML-Ausgabe durch die Verwendung von benutzerdefinierten CSS-Eigenschaften. |
| [setEncodeEntityAsCode(boolean value)](#setEncodeEntityAsCode-boolean-) | Gibt an, ob die HTML‑Zeichenentitäten durch dezimale Codes ersetzt werden. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Falls nicht festgelegt, wird Encoding.UTF8 als Standard‑Kodierungstyp verwendet. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | Gibt an, ob ungenutzte Stile ausgeschlossen werden. |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | Gibt an, ob Bilddateien in ein temporäres Verzeichnis exportiert werden. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Gibt an, ob nur das aktive Arbeitsblatt in eine HTML‑Datei exportiert wird. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Legt den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts fest. |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | Gibt an, ob fehlerhafte Daten der unteren Zeile exportiert werden. |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | Gibt an, ob beim Speichern der Datei als HTML die Excel‑Koordinaten nicht leerer Zellen exportiert werden. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Gibt an, ob Kommentare beim Speichern der Datei nach HTML exportiert werden; der Standardwert ist false. |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | Stellt den Typ des Exports von Kommentaren in HTML‑Dateien dar. |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | Gibt die Regel für den Export von HTML‑Dateidaten an. Der Standardwert ist Alle. |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger als die maximal anzeigbare Spalte ist. |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | Gibt an, ob Formeln beim Speichern der Datei als HTML exportiert werden. |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | Gibt an, ob Frame‑Skripte und Dokumenteigenschaften exportiert werden. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML‑Dateien exportiert werden. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Gibt an, ob der Inhalt ausgeblendeter Arbeitsblätter exportiert wird. Der Standardwert ist true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Legt fest, ob Bilder im Base64‑Format in HTML, MHTML oder EPUB gespeichert werden. |
| [setExportNamedRangeAnchors(boolean value)](#setExportNamedRangeAnchors-boolean-) | Gibt an, ob Anker‑Elemente für benannte Bereiche beim Speichern als HTML exportiert werden. |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | Legt den ExportObjectListener für das Exportieren von Objekten fest. |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | Gibt an, ob Seitenkopfzeilen exportiert werden. |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | Gibt an, ob Seitenkopfzeilen exportiert werden. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Gibt an, ob nur der Druckbereich in eine HTML‑Datei exportiert wird. |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML‑Dateien exportiert werden. |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | Gibt an, ob ein ähnlicher Rahmenstil exportiert wird, wenn der Rahmenstil von Browsern nicht unterstützt wird. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Gibt an, ob das einzelne Tabellenblatt exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | Gibt an, ob Arbeitsmappeneigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | Gibt an, ob das CSS des Arbeitsblatts separat exportiert wird. Der Standardwert ist false. |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | Gibt an, ob Arbeitsblatt‑Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei. |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | Legt den IFilePathProvider für das separate Exportieren von Arbeitsblättern nach HTML fest. |
| [setFormatDataIgnoreColumnWidth(boolean value)](#setFormatDataIgnoreColumnWidth-boolean-) | Gibt an, ob die vollständig formatierte Zellendaten angezeigt werden sollen, wenn die Spalte überläuft. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Gibt an, ob ein vollständiger Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | Versteckte Spalte (die Breite dieser Spalte ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird, wenn HtmlHiddenColDisplayType auf \"Remove\" gesetzt ist, wird die versteckte Spalte nicht ausgegeben; ist der Wert \"Hidden\", wird die Spalte ausgegeben, aber verborgen. Der Standardwert ist \"Hidden\". |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | Versteckte Zeile (die Höhe dieser Zeile ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird, wenn HtmlHiddenRowDisplayType auf \"Remove\" gesetzt ist, wird die versteckte Zeile nicht ausgegeben; ist der Wert \"Hidden\", wird die Zeile ausgegeben, aber verborgen. Der Standardwert ist \"Hidden\". |
| [setHideOverflowWrappedText(boolean value)](#setHideOverflowWrappedText-boolean-) | Gibt an, ob überlaufender Text ausgeblendet werden soll, wenn das Zellenformat auf Zeilenumbruch gesetzt ist. |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | Gibt an, ob ein über mehrere Zellen erstreckender Text beim Speichern einer Excel‑Datei im HTML‑Format auf dieselbe Weise wie in MS Excel angezeigt wird. |
| [setHtmlVersion(int value)](#setHtmlVersion-int-) | Gibt die HTML‑Standardversion an, die beim Speichern im HTML‑Format verwendet werden soll. |
| [setIECompatible(boolean value)](#setIECompatible-boolean-) | Gibt an, ob das ausgegebene HTML mit dem IE‑Browser kompatibel ist. |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | Gibt an, ob nicht sichtbare Formen exportiert werden. |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird, wenn eine skalierbare Einheit zur Beschreibung der Spaltenbreite verwendet wird. |
| [setJsBrowserCompatible(boolean value)](#setJsBrowserCompatible-boolean-) | Gibt an, ob JavaScript mit Browsern kompatibel ist, die kein JavaScript unterstützen. |
| [setLayoutMode(int value)](#setLayoutMode-int-) | Legt den Layout‑Modus beim Speichern nach HTML fest. |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | Gibt den Typ des target‑Attributs im `<a>`‑Link an. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden. |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | Gibt an, ob leere TD‑Elemente beim Exportieren der Datei nach HTML zwangsweise zusammengeführt werden. |
| [setMergeEmptyTdType(int value)](#setMergeEmptyTdType-int-) | Die Option, zusammenhängende leere Zellen (leere td‑Elemente) zusammenzuführen. Der Standardwert ist MergeEmptyTdType.Default. |
| [setMobileCompatible(boolean value)](#setMobileCompatible-boolean-) | Gibt an, ob das ausgegebene HTML mit mobilen Geräten kompatibel ist. |
| [setOfficeMathOutputMode(int value)](#setOfficeMathOutputMode-int-) | Gibt an, wie OfficeMath‑Objekte nach HTML exportiert werden. Der Standardwert ist Image. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | Der Titel der HTML‑Seite. |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Gibt an, ob HTML‑Tags (wie `<div></div>`) in einer Zelle als Zellwert geparst oder unverändert beibehalten werden sollen. |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Gibt an, ob HTML‑ oder MHT‑Datei die bevorzugte Darstellung ist. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen. |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | Gibt an, ob das HTML als einzelne Datei gespeichert werden soll. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Legt die zu rendernden Arbeitsblätter fest. |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | Gibt an, ob beim Speichern als einzelne HTML‑Datei alle Arbeitsblätter angezeigt werden. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden. |
| [setSpaceMode(int value)](#setSpaceMode-int-) | Gibt an, wie Leerzeichen in der HTML‑Ausgabe gerendert werden. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Legt den IStreamProvider für das Exportieren von Objekten fest. |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | Legt das Präfix des Typ‑CSS‑Namens fest, z. B. tr, col, td usw.; sie sind im Table‑Element enthalten, das das spezifische TableCssId‑Attribut besitzt. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Legt die Warn‑Callback‑Funktion fest. |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | Gibt an, ob die Spaltenbreite in Skalierungseinheiten nach HTML exportiert wird. |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | Gibt an, ob beim Speichern der Datei nach HTML über das Arbeitsblatt‑Zoomlevel in das HTML hinein- oder herausgezoomt wird; der Standardwert ist false. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Erstellt Optionen zum Speichern einer HTML-Datei.

### HtmlSaveOptions(int saveFormat) {#HtmlSaveOptions-int-}
```
public HtmlSaveOptions(int saveFormat)
```


Erstellt Optionen zum Speichern einer HTM-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Das Dateiformat. Es sollte einer der folgenden Typen sein: [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML) oder [SaveFormat.M\_HTML](../../com.aspose.cells/saveformat\#M-HTML), andernfalls wird das gespeicherte Format automatisch auf [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML) gesetzt. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAddGenericFont() {#getAddGenericFont--}
```
public boolean getAddGenericFont()
```


Gibt an, ob eine generische Schriftart zur CSS‑font-family hinzugefügt wird. Der Standardwert ist true.

**Returns:**
boolean
### getAddTooltipText() {#getAddTooltipText--}
```
public boolean getAddTooltipText()
```


Gibt an, ob ein Tooltip‑Text hinzugefügt wird, wenn die Daten nicht vollständig angezeigt werden können. Der Standardwert ist false.

**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. Nur beim Speichern in einen HTML‑Stream.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Gibt das URL‑Präfix für angehängte Dateien wie Bilder in der HTML‑Datei an. Nur beim Speichern in einen HTML‑Stream.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können.

**Remarks**

Wenn der Ordner nicht angegeben wurde, ist der Standardwert dafür [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Wenn sein Standardwert null oder leer ist oder als null oder leer angegeben wurde, wird beim Speichern der Arbeitsmappe keine Cache‑Datei verwendet.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Gibt an, ob Formeln vor dem Speichern der HTML-Datei berechnet werden sollen.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getCellCssPrefix() {#getCellCssPrefix--}
```
public String getCellCssPrefix()
```


Ermittelt das Präfix des CSS-Namens, der Standardwert ist "".

**Returns:**
java.lang.String
### getCellNameAttribute() {#getCellNameAttribute--}
```
public String getCellNameAttribute()
```


Gibt das Attribut an, das den zu schreibenden CellName angibt. (z. B. Wenn der Wert "id" ist, wird für die Zelle "A1" die Ausgabe <td id='A1'> sein). Der Standardwert ist null.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Ob die Beschränkungen einer Excel-Datei geprüft werden, wenn der Benutzer Zellen-bezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht das Eingeben eines Zeichenfolgenwerts, der länger als 32 K ist. Wenn Sie einen Wert eingeben, der länger als 32 K ist, wird er abgeschnitten.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Leert die Arbeitsmappe nach dem Speichern der Datei.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getCssStyles() {#getCssStyles--}
```
public String getCssStyles()
```


Ruft die zusätzlichen CSS‑Stile für den Formatter ab. Funktioniert nur, wenn [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) True ist.  CssStyles="body \{ padding: 5px \}";

**Returns:**
java.lang.String
### getDataBarRenderMode() {#getDataBarRenderMode--}
```
public int getDataBarRenderMode()
```


Stellt den Modus dar, wie DataBar beim Konvertieren von Excel‑Dateien in HTML‑Dateien gerendert wird. Der Standardwert ist [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

Siehe [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Geben Sie den Standard-Schriftartnamen für den Export von HTML an; die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null.

**Returns:**
java.lang.String
### getDisableCss() {#getDisableCss--}
```
public boolean getDisableCss()
```


Gibt an, ob nur Inline‑Stile angewendet werden, ohne sich auf CSS zu verlassen. Der Standardwert ist false.

**Returns:**
boolean
### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}
```
public boolean getDisableDownlevelRevealedComments()
```


Gibt an, ob Downlevel-revealed bedingte Kommentare beim Exportieren der Datei nach HTML deaktiviert werden; der Standardwert ist false.

**Returns:**
boolean
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


Ruft den Typ der Einbettung von Schriftartdateien in die HTML‑Datei ab. Der Standardwert ist [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE), was bedeutet, dass keine Schriftart in HTML eingebettet wird.

Siehe [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Returns:**
int
### getEnableCssCustomProperties() {#getEnableCssCustomProperties--}
```
public boolean getEnableCssCustomProperties()
```


Optimiert die HTML‑Ausgabe durch Verwendung von CSS‑benutzerdefinierten Eigenschaften. Zum Beispiel, wenn ein Base64‑Bild mehrfach vorkommt, muss mit einer benutzerdefinierten Eigenschaft das Bild nur einmal gespeichert werden, sodass die Leistung des resultierenden HTML verbessert werden kann. Der Standardwert ist false.

**Returns:**
boolean
### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}
```
public boolean getEncodeEntityAsCode()
```


Gibt an, ob HTML‑Zeichenentitäten durch dezimale Codes ersetzt werden. (z. B. "&nbsp;" wird durch "&\#160;" ersetzt). Der Standardwert ist false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Falls nicht festgelegt, wird Encoding.UTF8 als Standard‑Kodierungstyp verwendet.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.

**Remarks**

Nur für .xls, .xlsx, .xlsb und .xlsm-Dateien.

**Returns:**
boolean
### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}
```
public boolean getExcludeUnusedStyles()
```


Gibt an, ob ungenutzte Stile ausgeschlossen werden. Für die erzeugten HTML‑Dateien kann das Ausschließen ungenutzter Stile die Dateigröße verkleinern, ohne die visuellen Effekte zu beeinträchtigen. Daher ist der Standardwert dieser Eigenschaft true. Wenn der Benutzer alle Stile in der Arbeitsmappe für das erzeugte HTML beibehalten muss (z. B. wenn die Arbeitsmappe später aus dem erzeugten HTML wiederhergestellt werden soll), setzen Sie diese Eigenschaft bitte auf false.

**Returns:**
boolean
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Gibt an, ob nur das aktive Arbeitsblatt in eine HTML‑Datei exportiert wird. Wenn true, wird nur das aktive Arbeitsblatt in die HTML‑Datei exportiert; wenn false, wird die gesamte Arbeitsmappe in die HTML‑Datei exportiert. Der Standardwert ist false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Ruft den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts ab. Wenn Sie dieses Attribut setzen, wird der Druckbereich des aktuell aktiven Arbeitsblatts weggelassen. Beim Speichern der Datei als HTML wird nur der angegebene Bereich exportiert.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportBogusRowData() {#getExportBogusRowData--}
```
public boolean getExportBogusRowData()
```


Gibt an, ob falsche Daten der unteren Zeile exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Returns:**
boolean
### getExportCellCoordinate() {#getExportCellCoordinate--}
```
public boolean getExportCellCoordinate()
```


Gibt an, ob beim Speichern der Datei als HTML die Excel‑Koordinaten nicht leerer Zellen exportiert werden. Der Standardwert ist false. Wenn Sie das erzeugte HTML in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Returns:**
boolean
### getExportCommentsType() {#getExportCommentsType--}
```
public int getExportCommentsType()
```


Stellt den Typ des Exports von Kommentaren in HTML‑Dateien dar.

Siehe [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getExportDataOptions() {#getExportDataOptions--}
```
public int getExportDataOptions()
```


Gibt die Regel für den Export von HTML‑Dateidaten an. Der Standardwert ist Alle.

Siehe [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Returns:**
int
### getExportDocumentProperties() {#getExportDocumentProperties--}
```
public boolean getExportDocumentProperties()
```


Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Returns:**
boolean
### getExportExtraHeadings() {#getExportExtraHeadings--}
```
public boolean getExportExtraHeadings()
```


Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger ist als die maximal anzeigbare Spalte. Der Standardwert ist false. Wenn Sie die HTML‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Returns:**
boolean
### getExportFormula() {#getExportFormula--}
```
public boolean getExportFormula()
```


Gibt an, ob Formeln beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist true. Wenn Sie das exportierte HTML in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Returns:**
boolean
### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}
```
public boolean getExportFrameScriptsAndProperties()
```


Gibt an, ob Frame‑Skripte und Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Returns:**
boolean
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML‑Dateien exportiert werden.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft HtmlSaveOptions.ExportRowColumnHeadings. Diese Eigenschaft wird 12 Monate nach Juni 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Gibt an, ob der Inhalt ausgeblendeter Arbeitsblätter exportiert wird. Der Standardwert ist true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Legt fest, ob Bilder im Base64‑Format in HTML, MHTML oder EPUB gespeichert werden.

**Remarks**

Wenn diese Eigenschaft auf true gesetzt ist, werden Bilddaten direkt in den img‑Elementen exportiert und separate Dateien werden nicht erstellt.

**Returns:**
boolean
### getExportNamedRangeAnchors() {#getExportNamedRangeAnchors--}
```
public boolean getExportNamedRangeAnchors()
```


Gibt an, ob Anker‑Elemente für benannte Bereiche beim Speichern als HTML exportiert werden. Der Standardwert ist true.

**Returns:**
boolean
### getExportObjectListener() {#getExportObjectListener--}
```
public IExportObjectListener getExportObjectListener()
```


Ruft den ExportObjectListener für den Export von Objekten ab.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft HtmlSaveOptions.IStreamProvider. Diese Eigenschaft wird 12 Monate nach August 2015 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
[IExportObjectListener](../../com.aspose.cells/iexportobjectlistener)
### getExportPageFooters() {#getExportPageFooters--}
```
public boolean getExportPageFooters()
```


Gibt an, ob Seitenkopfzeilen exportiert werden.

**Remarks**

Funktioniert nur, wenn [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) True ist.

**Returns:**
boolean
### getExportPageHeaders() {#getExportPageHeaders--}
```
public boolean getExportPageHeaders()
```


Gibt an, ob Seitenkopfzeilen exportiert werden.

**Remarks**

Funktioniert nur, wenn [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) True ist.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Gibt an, ob nur der Druckbereich in die HTML‑Datei exportiert wird. Der Standardwert ist false.

**Returns:**
boolean
### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}
```
public boolean getExportRowColumnHeadings()
```


Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML‑Dateien exportiert werden.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}
```
public boolean getExportSimilarBorderStyle()
```


Gibt an, ob ein ähnlicher Rahmenstil exportiert wird, wenn der Rahmenstil von Browsern nicht unterstützt wird. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. Der Standardwert ist false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Gibt an, ob das einzelne Tabellenblatt exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. Der Standardwert ist false.

**Returns:**
boolean
### getExportWorkbookProperties() {#getExportWorkbookProperties--}
```
public boolean getExportWorkbookProperties()
```


Gibt an, ob Arbeitsmappeneigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Returns:**
boolean
### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}
```
public boolean getExportWorksheetCSSSeparately()
```


Gibt an, ob das CSS des Arbeitsblatts separat exportiert wird. Der Standardwert ist false.

**Returns:**
boolean
### getExportWorksheetProperties() {#getExportWorksheetProperties--}
```
public boolean getExportWorksheetProperties()
```


Gibt an, ob Arbeitsblatt‑Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Returns:**
boolean
### getFilePathProvider() {#getFilePathProvider--}
```
public IFilePathProvider getFilePathProvider()
```


Ruft den IFilePathProvider zum separaten Exportieren des Arbeitsblatts nach HTML ab.

**Returns:**
[IFilePathProvider](../../com.aspose.cells/ifilepathprovider)
### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}
```
public boolean getFormatDataIgnoreColumnWidth()
```


Gibt an, ob die vollständig formatierte Zellendaten angezeigt werden, wenn der Inhalt die Spalte überläuft. Wenn true, wird die Spaltenbreite ignoriert und die gesamten Zellendaten werden exportiert. Wenn false, werden die Daten wie in Excel exportiert. Der Standardwert ist false.

**Returns:**
boolean
### getHiddenColDisplayType() {#getHiddenColDisplayType--}
```
public int getHiddenColDisplayType()
```


Versteckte Spalte (die Breite dieser Spalte ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird, wenn HtmlHiddenColDisplayType auf \"Remove\" gesetzt ist, wird die versteckte Spalte nicht ausgegeben; ist der Wert \"Hidden\", wird die Spalte ausgegeben, aber verborgen. Der Standardwert ist \"Hidden\".

Siehe [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Returns:**
int
### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}
```
public int getHiddenRowDisplayType()
```


Versteckte Zeile (die Höhe dieser Zeile ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird, wenn HtmlHiddenRowDisplayType auf \"Remove\" gesetzt ist, wird die versteckte Zeile nicht ausgegeben; ist der Wert \"Hidden\", wird die Zeile ausgegeben, aber verborgen. Der Standardwert ist \"Hidden\".

Siehe [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Returns:**
int
### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}
```
public boolean getHideOverflowWrappedText()
```


Gibt an, ob überlaufender Text ausgeblendet wird, wenn das Zellenformat auf Zeilenumbruch gesetzt ist. Der Standardwert ist false

**Returns:**
boolean
### getHtmlCrossStringType() {#getHtmlCrossStringType--}
```
public int getHtmlCrossStringType()
```


Gibt an, ob ein über mehrere Zellen erstreckender Text beim Speichern einer Excel‑Datei im HTML‑Format auf dieselbe Weise wie MS Excel angezeigt wird. Standardmäßig ist der Wert Default, sodass es bei über Zellen erstreckenden Zeichenketten kaum Unterschiede zwischen den von Aspose.Cells und MS Excel erstellten HTML‑Dateien gibt. Die Leistung beim Erstellen großer HTML‑Dateien ist jedoch mehrere Male höher, wenn der Wert auf Cross gesetzt wird, im Vergleich zu Default oder Fit2Cell.

Siehe [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Returns:**
int
### getHtmlVersion() {#getHtmlVersion--}
```
public int getHtmlVersion()
```


Gibt die Version des HTML‑Standards an, die beim Speichern im HTML‑Format verwendet werden soll. Der Standardwert ist HtmlVersion.Default.

Siehe [HtmlVersion](../../com.aspose.cells/htmlversion).

**Returns:**
int
### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}
```
public boolean getIgnoreInvisibleShapes()
```


Gibt an, ob nicht sichtbare Formen exportiert werden.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Rufen Sie das ImageOrPrintOptions‑Objekt vor dem Exportieren ab.

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getImageScalable() {#getImageScalable--}
```
public boolean getImageScalable()
```


Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird, wenn eine skalierbare Einheit zur Beschreibung der Spaltenbreite verwendet wird. Der Standardwert ist true.

**Returns:**
boolean
### getLayoutMode() {#getLayoutMode--}
```
public int getLayoutMode()
```


Ermittelt den Layoutmodus beim Speichern als HTML. Der Standardwert ist [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Siehe [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Returns:**
int
### getLinkTargetType() {#getLinkTargetType--}
```
public int getLinkTargetType()
```


Gibt den Typ des target-Attributs in einem `<a>`-Link an. Der Standardwert ist HtmlLinkTargetType.Parent.

Siehe [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Returns:**
int
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}
```
public boolean getMergeEmptyTdForcely()
```


Gibt an, ob leere TD-Elemente beim Exportieren der Datei nach HTML zwangsweise zusammengeführt werden. Die Dateigröße von HTML wird nach dem Setzen des Werts auf true deutlich reduziert. Der Standardwert ist false. Wenn Sie die HTML-Datei nach Excel importieren oder beim Speichern der Datei nach HTML perfekte Gitternetzlinien exportieren möchten, behalten Sie bitte den Standardwert bei.

**Returns:**
boolean
### getMergeEmptyTdType() {#getMergeEmptyTdType--}
```
public int getMergeEmptyTdType()
```


Die Option, zusammenhängende leere Zellen (leere td‑Elemente) zusammenzuführen. Der Standardwert ist MergeEmptyTdType.Default.

Siehe [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Returns:**
int
### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}
```
public int getOfficeMathOutputMode()
```


Gibt an, wie OfficeMath‑Objekte nach HTML exportiert werden. Der Standardwert ist Image.

Siehe [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Returns:**
int
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


Der Titel der HTML-Seite. Nur beim Speichern in einen HTML-Stream.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Gibt an, ob HTML-Tags (wie `<div></div>`) in einer Zelle als Zellenwert geparst oder unverändert beibehalten werden sollen. Der Standardwert ist true.

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Gibt an, ob HTML- oder MHT-Datei die bevorzugte Darstellung ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung erhalten möchten, setzen Sie den Wert bitte auf true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.

**Returns:**
boolean
### getSaveAsSingleFile() {#getSaveAsSingleFile--}
```
public boolean getSaveAsSingleFile()
```


Gibt an, ob das HTML als einzelne Datei gespeichert wird. Der Standardwert ist false.

**Remarks**

Wenn das Arbeitsbuch mehrere Arbeitsblätter oder andere erforderliche Ressourcen wie Bilder enthält, müssen diese Arbeitsblätter und Ressourcen normalerweise in separaten Dateien gespeichert werden. Für einige Szenarien benötigt der Benutzer möglicherweise nur eine einzige Ergebnisdatei, z. B. zum einfachen Übertragen. In diesem Fall kann der Benutzer diese Eigenschaft auf true setzen.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ermittelt das Speicherdateiformat.

Siehe [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Ermittelt die zu rendernden Arbeitsblätter. Standard ist jedes sichtbare Arbeitsblatt im Arbeitsbuch: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getShowAllSheets() {#getShowAllSheets--}
```
public boolean getShowAllSheets()
```


Gibt an, ob beim Speichern als einzelne HTML‑Datei alle Arbeitsblätter angezeigt werden.

**Remarks**

Funktioniert nur, wenn [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) True ist.

**Returns:**
boolean
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.

**Returns:**
boolean
### getSpaceMode() {#getSpaceMode--}
```
public int getSpaceMode()
```


Gibt an, wie Leerzeichen in der HTML-Ausgabe gerendert werden. Diese Option wird derzeit nur bei numerischen Formaten (z. B. Buchhaltungsformat) angewendet. Der Standardwert ist [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Siehe [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Returns:**
int
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Ruft den IStreamProvider zum Exportieren von Objekten ab.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```


Ermittelt das Präfix des CSS-Typs, wie tr, col, td usw., die im Table-Element mit dem spezifischen TableCssId-Attribut enthalten sind. Der Standardwert ist "".

**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Gibt an, ob die Smart‑Art‑Einstellung aktualisiert wird. Der Standardwert ist false.

**Remarks**

Wirkt nur nach dem Aufruf der Methode Shape.GetResultOfSmartArt() und wenn die zwischengespeicherten Shapes in der Vorlagendatei vorhanden sind.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.

**Remarks**

Der Standardwert ist false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Liest den Warn‑Callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWidthScalable() {#getWidthScalable--}
```
public boolean getWidthScalable()
```


Gibt an, ob die Spaltenbreite in Skalareinheiten nach HTML exportiert wird. Der Standardwert ist false.

**Returns:**
boolean
### getWorksheetScalable() {#getWorksheetScalable--}
```
public boolean getWorksheetScalable()
```


Gibt an, ob beim Speichern der Datei nach HTML über das Arbeitsblatt‑Zoomlevel in das HTML hinein- oder herausgezoomt wird; der Standardwert ist false.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBorderCollapsed() {#isBorderCollapsed--}
```
public boolean isBorderCollapsed()
```


Gibt an, ob die Tabellenränder zusammengeführt werden. Der Standardwert ist true.

**Returns:**
boolean
### isExpImageToTempDir() {#isExpImageToTempDir--}
```
public boolean isExpImageToTempDir()
```


Gibt an, ob Bilddateien in ein temporäres Verzeichnis exportiert werden. Nur beim Speichern in einen HTML-Stream.

**Returns:**
boolean
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Gibt an, ob Kommentare beim Speichern der Datei nach HTML exportiert werden; der Standardwert ist false.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Gibt an, ob ein vollständiger Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. Der Standardwert ist false.

**Returns:**
boolean
### isIECompatible() {#isIECompatible--}
```
public boolean isIECompatible()
```


Gibt an, ob das ausgegebene HTML mit dem IE-Browser kompatibel ist. Der Standardwert ist false

**Returns:**
boolean
### isJsBrowserCompatible() {#isJsBrowserCompatible--}
```
public boolean isJsBrowserCompatible()
```


Gibt an, ob JavaScript mit Browsern kompatibel ist, die kein JavaScript unterstützen. Der Standardwert ist true.

**Returns:**
boolean
### isMobileCompatible() {#isMobileCompatible--}
```
public boolean isMobileCompatible()
```


Gibt an, ob das ausgegebene HTML mit mobilen Geräten kompatibel ist. Der Standardwert ist false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAddGenericFont(boolean value) {#setAddGenericFont-boolean-}
```
public void setAddGenericFont(boolean value)
```


Gibt an, ob eine generische Schriftart zur CSS‑font-family hinzugefügt wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAddTooltipText(boolean value) {#setAddTooltipText-boolean-}
```
public void setAddTooltipText(boolean value)
```


Gibt an, ob ein Tooltip‑Text hinzugefügt wird, wenn die Daten nicht vollständig angezeigt werden können. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Das Verzeichnis, in dem die angehängten Dateien gespeichert werden. Nur beim Speichern in einen HTML‑Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Gibt das URL‑Präfix für angehängte Dateien wie Bilder in der HTML‑Datei an. Nur beim Speichern in einen HTML‑Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setBorderCollapsed(boolean value) {#setBorderCollapsed-boolean-}
```
public void setBorderCollapsed(boolean value)
```


Gibt an, ob die Tabellenränder zusammengeführt werden. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Der Ordner für temporäre Dateien, die als Daten-Cache verwendet werden können.

**Remarks**

Wenn der Ordner nicht angegeben wurde, ist der Standardwert dafür [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Wenn sein Standardwert null oder leer ist oder als null oder leer angegeben wurde, wird beim Speichern der Arbeitsmappe keine Cache‑Datei verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Gibt an, ob Formeln vor dem Speichern der HTML-Datei berechnet werden sollen.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```


Legt das Präfix des CSS‑Namens fest, der Standardwert ist "".

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCellNameAttribute(String value) {#setCellNameAttribute-java.lang.String-}
```
public void setCellNameAttribute(String value)
```


Gibt das Attribut an, das den zu schreibenden CellName angibt. (z. B. Wenn der Wert "id" ist, wird für die Zelle "A1" die Ausgabe <td id='A1'> sein). Der Standardwert ist null.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Ob die Beschränkungen einer Excel-Datei geprüft werden, wenn der Benutzer Zellen-bezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht das Eingeben eines Zeichenfolgenwerts, der länger als 32 K ist. Wenn Sie einen Wert eingeben, der länger als 32 K ist, wird er abgeschnitten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Leert die Arbeitsmappe nach dem Speichern der Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCssStyles(String value) {#setCssStyles-java.lang.String-}
```
public void setCssStyles(String value)
```


Legt die zusätzlichen CSS‑Stile für den Formatter fest. Funktioniert nur, wenn [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) True ist.  CssStyles="body \{ padding: 5px \}";

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDataBarRenderMode(int value) {#setDataBarRenderMode-int-}
```
public void setDataBarRenderMode(int value)
```


Stellt den Modus dar, wie DataBar beim Konvertieren von Excel‑Dateien in HTML‑Dateien gerendert wird. Der Standardwert ist [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

Siehe [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Geben Sie den Standard-Schriftartnamen für den Export von HTML an; die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDisableCss(boolean value) {#setDisableCss-boolean-}
```
public void setDisableCss(boolean value)
```


Gibt an, ob nur Inline‑Stile angewendet werden, ohne sich auf CSS zu verlassen. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```


Gibt an, ob Downlevel-revealed bedingte Kommentare beim Exportieren der Datei nach HTML deaktiviert werden; der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


Legt den Typ der eingebetteten Schriftdatei in die HTML‑Datei fest. Der Standardwert ist [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE), was bedeutet, dass keine Schrift in HTML eingebettet wird.

Siehe [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setEnableCssCustomProperties(boolean value) {#setEnableCssCustomProperties-boolean-}
```
public void setEnableCssCustomProperties(boolean value)
```


Optimiert die HTML‑Ausgabe durch Verwendung von CSS‑benutzerdefinierten Eigenschaften. Zum Beispiel, wenn ein Base64‑Bild mehrfach vorkommt, muss mit einer benutzerdefinierten Eigenschaft das Bild nur einmal gespeichert werden, sodass die Leistung des resultierenden HTML verbessert werden kann. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEncodeEntityAsCode(boolean value) {#setEncodeEntityAsCode-boolean-}
```
public void setEncodeEntityAsCode(boolean value)
```


Gibt an, ob HTML‑Zeichenentitäten durch dezimale Codes ersetzt werden. (z. B. "&nbsp;" wird durch "&\#160;" ersetzt). Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Falls nicht festgelegt, wird Encoding.UTF8 als Standard‑Kodierungstyp verwendet.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.

**Remarks**

Nur für .xls, .xlsx, .xlsb und .xlsm-Dateien.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```


Gibt an, ob ungenutzte Stile ausgeschlossen werden. Für die erzeugten HTML‑Dateien kann das Ausschließen ungenutzter Stile die Dateigröße verkleinern, ohne die visuellen Effekte zu beeinträchtigen. Daher ist der Standardwert dieser Eigenschaft true. Wenn der Benutzer alle Stile in der Arbeitsmappe für das erzeugte HTML beibehalten muss (z. B. wenn die Arbeitsmappe später aus dem erzeugten HTML wiederhergestellt werden soll), setzen Sie diese Eigenschaft bitte auf false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```


Gibt an, ob Bilddateien in ein temporäres Verzeichnis exportiert werden. Nur beim Speichern in einen HTML-Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Gibt an, ob nur das aktive Arbeitsblatt in eine HTML‑Datei exportiert wird. Wenn true, wird nur das aktive Arbeitsblatt in die HTML‑Datei exportiert; wenn false, wird die gesamte Arbeitsmappe in die HTML‑Datei exportiert. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Legt den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts fest. Wenn Sie dieses Attribut setzen, wird der Druckbereich des aktuell aktiven Arbeitsblatts weggelassen. Beim Speichern der Datei als HTML wird nur der angegebene Bereich exportiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```


Gibt an, ob falsche Daten der unteren Zeile exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```


Gibt an, ob beim Speichern der Datei als HTML die Excel‑Koordinaten nicht leerer Zellen exportiert werden. Der Standardwert ist false. Wenn Sie das erzeugte HTML in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Gibt an, ob Kommentare beim Speichern der Datei nach HTML exportiert werden; der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```


Stellt den Typ des Exports von Kommentaren in HTML‑Dateien dar.

Siehe [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```


Gibt die Regel für den Export von HTML‑Dateidaten an. Der Standardwert ist Alle.

Siehe [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```


Gibt an, ob Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```


Gibt an, ob zusätzliche Überschriften exportiert werden, wenn die Textlänge länger ist als die maximal anzeigbare Spalte. Der Standardwert ist false. Wenn Sie die HTML‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```


Gibt an, ob Formeln beim Speichern der Datei als HTML exportiert werden. Der Standardwert ist true. Wenn Sie das exportierte HTML in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```


Gibt an, ob Frame‑Skripte und Dokumenteigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Gibt an, ob Rasterlinien exportiert werden. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML‑Dateien exportiert werden.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft HtmlSaveOptions.ExportRowColumnHeadings. Diese Eigenschaft wird 12 Monate nach Juni 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Gibt an, ob der Inhalt ausgeblendeter Arbeitsblätter exportiert wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Legt fest, ob Bilder im Base64‑Format in HTML, MHTML oder EPUB gespeichert werden.

**Remarks**

Wenn diese Eigenschaft auf true gesetzt ist, werden Bilddaten direkt in den img‑Elementen exportiert und separate Dateien werden nicht erstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportNamedRangeAnchors(boolean value) {#setExportNamedRangeAnchors-boolean-}
```
public void setExportNamedRangeAnchors(boolean value)
```


Gibt an, ob Anker‑Elemente für benannte Bereiche beim Speichern als HTML exportiert werden. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```


Legt den ExportObjectListener für das Exportieren von Objekten fest.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die Eigenschaft HtmlSaveOptions.IStreamProvider. Diese Eigenschaft wird 12 Monate nach August 2015 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |

### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```


Gibt an, ob Seitenkopfzeilen exportiert werden.

**Remarks**

Funktioniert nur, wenn [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) True ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```


Gibt an, ob Seitenkopfzeilen exportiert werden.

**Remarks**

Funktioniert nur, wenn [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) True ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Gibt an, ob nur der Druckbereich in die HTML‑Datei exportiert wird. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```


Gibt an, ob Zeilen‑ und Spaltenüberschriften des Blatts beim Speichern in HTML‑Dateien exportiert werden.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```


Gibt an, ob ein ähnlicher Rahmenstil exportiert wird, wenn der Rahmenstil von Browsern nicht unterstützt wird. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Gibt an, ob das einzelne Tabellenblatt exportiert wird, wenn die Datei nur ein Arbeitsblatt enthält. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```


Gibt an, ob Arbeitsmappeneigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei in Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```


Gibt an, ob das CSS des Arbeitsblatts separat exportiert wird. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```


Gibt an, ob Arbeitsblatt‑Eigenschaften exportiert werden. Der Standardwert ist true. Wenn Sie die HTML‑ oder MHT‑Datei nach Excel importieren möchten, behalten Sie bitte den Standardwert bei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```


Legt den IFilePathProvider für das separate Exportieren von Arbeitsblättern nach HTML fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |

### setFormatDataIgnoreColumnWidth(boolean value) {#setFormatDataIgnoreColumnWidth-boolean-}
```
public void setFormatDataIgnoreColumnWidth(boolean value)
```


Gibt an, ob die vollständig formatierte Zellendaten angezeigt werden, wenn der Inhalt die Spalte überläuft. Wenn true, wird die Spaltenbreite ignoriert und die gesamten Zellendaten werden exportiert. Wenn false, werden die Daten wie in Excel exportiert. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Gibt an, ob ein vollständiger Pfadlink in sheet00x.htm, filelist.xml und tabstrip.htm verwendet wird. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```


Versteckte Spalte (die Breite dieser Spalte ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird, wenn HtmlHiddenColDisplayType auf \"Remove\" gesetzt ist, wird die versteckte Spalte nicht ausgegeben; ist der Wert \"Hidden\", wird die Spalte ausgegeben, aber verborgen. Der Standardwert ist \"Hidden\".

Siehe [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```


Versteckte Zeile (die Höhe dieser Zeile ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird, wenn HtmlHiddenRowDisplayType auf \"Remove\" gesetzt ist, wird die versteckte Zeile nicht ausgegeben; ist der Wert \"Hidden\", wird die Zeile ausgegeben, aber verborgen. Der Standardwert ist \"Hidden\".

Siehe [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHideOverflowWrappedText(boolean value) {#setHideOverflowWrappedText-boolean-}
```
public void setHideOverflowWrappedText(boolean value)
```


Gibt an, ob überlaufender Text ausgeblendet wird, wenn das Zellenformat auf Zeilenumbruch gesetzt ist. Der Standardwert ist false

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```


Gibt an, ob ein über mehrere Zellen erstreckender Text beim Speichern einer Excel‑Datei im HTML‑Format auf dieselbe Weise wie MS Excel angezeigt wird. Standardmäßig ist der Wert Default, sodass es bei über Zellen erstreckenden Zeichenketten kaum Unterschiede zwischen den von Aspose.Cells und MS Excel erstellten HTML‑Dateien gibt. Die Leistung beim Erstellen großer HTML‑Dateien ist jedoch mehrere Male höher, wenn der Wert auf Cross gesetzt wird, im Vergleich zu Default oder Fit2Cell.

Siehe [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHtmlVersion(int value) {#setHtmlVersion-int-}
```
public void setHtmlVersion(int value)
```


Gibt die Version des HTML‑Standards an, die beim Speichern im HTML‑Format verwendet werden soll. Der Standardwert ist HtmlVersion.Default.

Siehe [HtmlVersion](../../com.aspose.cells/htmlversion).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setIECompatible(boolean value) {#setIECompatible-boolean-}
```
public void setIECompatible(boolean value)
```


Gibt an, ob das ausgegebene HTML mit dem IE-Browser kompatibel ist. Der Standardwert ist false

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```


Gibt an, ob nicht sichtbare Formen exportiert werden.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```


Gibt an, ob eine skalierbare Einheit zur Beschreibung der Bildbreite verwendet wird, wenn eine skalierbare Einheit zur Beschreibung der Spaltenbreite verwendet wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setJsBrowserCompatible(boolean value) {#setJsBrowserCompatible-boolean-}
```
public void setJsBrowserCompatible(boolean value)
```


Gibt an, ob JavaScript mit Browsern kompatibel ist, die kein JavaScript unterstützen. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLayoutMode(int value) {#setLayoutMode-int-}
```
public void setLayoutMode(int value)
```


Legt den Layoutmodus beim Speichern als HTML fest. Der Standardwert ist [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Siehe [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```


Gibt den Typ des target-Attributs in einem `<a>`-Link an. Der Standardwert ist HtmlLinkTargetType.Parent.

Siehe [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```


Gibt an, ob leere TD-Elemente beim Exportieren der Datei nach HTML zwangsweise zusammengeführt werden. Die Dateigröße von HTML wird nach dem Setzen des Werts auf true deutlich reduziert. Der Standardwert ist false. Wenn Sie die HTML-Datei nach Excel importieren oder beim Speichern der Datei nach HTML perfekte Gitternetzlinien exportieren möchten, behalten Sie bitte den Standardwert bei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setMergeEmptyTdType(int value) {#setMergeEmptyTdType-int-}
```
public void setMergeEmptyTdType(int value)
```


Die Option, zusammenhängende leere Zellen (leere td‑Elemente) zusammenzuführen. Der Standardwert ist MergeEmptyTdType.Default.

Siehe [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMobileCompatible(boolean value) {#setMobileCompatible-boolean-}
```
public void setMobileCompatible(boolean value)
```


Gibt an, ob das ausgegebene HTML mit mobilen Geräten kompatibel ist. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOfficeMathOutputMode(int value) {#setOfficeMathOutputMode-int-}
```
public void setOfficeMathOutputMode(int value)
```


Gibt an, wie OfficeMath‑Objekte nach HTML exportiert werden. Der Standardwert ist Image.

Siehe [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


Der Titel der HTML-Seite. Nur beim Speichern in einen HTML-Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Gibt an, ob HTML-Tags (wie `<div></div>`) in einer Zelle als Zellenwert geparst oder unverändert beibehalten werden sollen. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Gibt an, ob HTML- oder MHT-Datei die bevorzugte Darstellung ist. Der Standardwert ist false. Wenn Sie eine schönere Darstellung erhalten möchten, setzen Sie den Wert bitte auf true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```


Gibt an, ob das HTML als einzelne Datei gespeichert wird. Der Standardwert ist false.

**Remarks**

Wenn das Arbeitsbuch mehrere Arbeitsblätter oder andere erforderliche Ressourcen wie Bilder enthält, müssen diese Arbeitsblätter und Ressourcen normalerweise in separaten Dateien gespeichert werden. Für einige Szenarien benötigt der Benutzer möglicherweise nur eine einzige Ergebnisdatei, z. B. zum einfachen Übertragen. In diesem Fall kann der Benutzer diese Eigenschaft auf true setzen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Legt die zu rendernden Arbeitsblätter fest. Standard ist, dass alle sichtbaren Arbeitsblätter in der Arbeitsmappe verwendet werden: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```


Gibt an, ob beim Speichern als einzelne HTML‑Datei alle Arbeitsblätter angezeigt werden.

**Remarks**

Funktioniert nur, wenn [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) True ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSpaceMode(int value) {#setSpaceMode-int-}
```
public void setSpaceMode(int value)
```


Gibt an, wie Leerzeichen in der HTML-Ausgabe gerendert werden. Diese Option wird derzeit nur bei numerischen Formaten (z. B. Buchhaltungsformat) angewendet. Der Standardwert ist [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Siehe [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Legt den IStreamProvider für das Exportieren von Objekten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```


Legt das Präfix des CSS‑Namenstyps fest, z. B. tr, col, td usw., die im Table‑Element enthalten sind, das das spezifische TableCssId‑Attribut besitzt. Der Standardwert ist "".

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Gibt an, ob die Smart‑Art‑Einstellung aktualisiert wird. Der Standardwert ist false.

**Remarks**

Wirkt nur nach dem Aufruf der Methode Shape.GetResultOfSmartArt() und wenn die zwischengespeicherten Shapes in der Vorlagendatei vorhanden sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.

**Remarks**

Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Legt die Warn‑Callback‑Funktion fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWidthScalable(boolean value) {#setWidthScalable-boolean-}
```
public void setWidthScalable(boolean value)
```


Gibt an, ob die Spaltenbreite in Skalareinheiten nach HTML exportiert wird. Der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```


Gibt an, ob beim Speichern der Datei nach HTML über das Arbeitsblatt‑Zoomlevel in das HTML hinein- oder herausgezoomt wird; der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

