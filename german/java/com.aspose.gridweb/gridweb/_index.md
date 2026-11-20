---
title: "GridWeb"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Die Grundklasse des GridWeb-Steuerelements."
type: docs
url: /de/java/com.aspose.gridweb/gridweb/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebControl](../../com.aspose.gridweb/webcontrol), [com.aspose.gridweb.ExtWebControl](../../com.aspose.gridweb/extwebcontrol), [com.aspose.gridweb.MainWeb](../../com.aspose.gridweb/mainweb)
```
public class GridWeb extends MainWeb
```

Die Grundklasse des GridWeb-Steuerelements.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GridWeb()](#GridWeb--) |  |
## Felder

| Feld | Beschreibung |
| --- | --- |
| [AfterColumnFilter](#AfterColumnFilter) | Tritt auf, nachdem die Spalte gefiltert wurde. |
| [AjaxCallFinished](#AjaxCallFinished) | Wird ausgelöst, wenn das Ajax-Update der Steuerung abgeschlossen ist. |
| [BeforeColumnFilter](#BeforeColumnFilter) | Tritt auf, bevor die Spalte gefiltert wird. |
| [CellClickOnAjax](#CellClickOnAjax) | Tritt auf, wenn die Zelle angeklickt wird, und erfordert einen Ajax-Callback für dieses Ereignis. |
| [CellClientUpdate](#CellClientUpdate) | Tritt auf, wenn ein Client-Zellen-Update stattfindet. |
| [CellCommand](#CellCommand) | Tritt auf, wenn der Befehls-Hyperlink einer Zelle angeklickt wird. |
| [CellDoubleClick](#CellDoubleClick) | Tritt auf, wenn die Zelle doppelt angeklickt wird. |
| [CellModifiedOnAjax](#CellModifiedOnAjax) | Tritt auf, wenn die Zelle in einem Ajax-Aufruf geändert wird. |
| [ColumnDeleted](#ColumnDeleted) | Tritt auf, wenn ein Benutzer eine Spalte über das clientseitige Menü löscht. |
| [ColumnDeleting](#ColumnDeleting) | Tritt auf, wenn ein Benutzer versucht, eine Spalte über das clientseitige Menü zu löschen. |
| [ColumnDoubleClick](#ColumnDoubleClick) | Tritt auf, wenn die Spaltenüberschrift doppelt angeklickt wird. |
| [ColumnInserted](#ColumnInserted) | Tritt auf, wenn ein Benutzer eine Spalte über das clientseitige Menü einfügt. |
| [CustomCommand](#CustomCommand) | Tritt auf, wenn ein Benutzer eine benutzerdefinierte Befehls-Schaltfläche anklickt. |
| [LoadCustomData](#LoadCustomData) | Wird ausgelöst, wenn der SessionMode der Steuerung auf Benutzerdefiniert gesetzt ist und Tabellendaten geladen werden müssen. |
| [PageIndexChanged](#PageIndexChanged) | Tritt auf, wenn sich der Blattseitenindex der Steuerung ändert. |
| [RowDeleted](#RowDeleted) | Tritt auf, wenn ein Benutzer eine Zeile über das clientseitige Menü gelöscht hat. |
| [RowDeleting](#RowDeleting) | Tritt auf, wenn ein Benutzer versucht, eine Zeile über das clientseitige Menü zu löschen. |
| [RowDoubleClick](#RowDoubleClick) | Tritt auf, wenn die Zeilenüberschrift doppelt angeklickt wird. |
| [RowInserted](#RowInserted) | Tritt auf, wenn ein Benutzer eine Zeile über das clientseitige Menü einfügt. |
| [SaveCommand](#SaveCommand) | Tritt auf, wenn die Schaltfläche "Speichern" angeklickt wird. |
| [SheetAdded](#SheetAdded) | Tritt auf, wenn ein Benutzer ein Arbeitsblatt über das Symbolleistenmenü hinzufügt. |
| [SheetTabClick](#SheetTabClick) | Tritt auf, wenn das Blattregister angeklickt wird. |
| [SubmitCommand](#SubmitCommand) | Tritt auf, wenn die Schaltfläche "Absenden" angeklickt wird. |
| [UndoCommand](#UndoCommand) | Tritt auf, wenn die Schaltfläche "Rückgängig" angeklickt wird. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [calculateFormula()](#calculateFormula--) | Berechnet das Ergebnis von Formeln. |
| [createChildControls()](#createChildControls--) | Implementiert CreateChildControls von WebControl, nur intern verwendet. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getACWClientPath()](#getACWClientPath--) | Ermittelt den Webpfad der Skript-/Bilddateien der Steuerung. |
| [getACWLanguageFileUrl()](#getACWLanguageFileUrl--) | Ermittelt die Web-URL der Sprachdatei der Steuerung. |
| [getActiveCell()](#getActiveCell--) | Ermittelt die aktive Zelle des aktuellen Blatts. |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | Legt die Hintergrundfarbe der aktiven Zelle fest. |
| [getActiveCellColor()](#getActiveCellColor--) | Legt die Farbe der aktiven Zelle fest. |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | Legt die Hintergrundfarbe der aktiven Zeilen-/Spaltenüberschrift fest. |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | Legt die Farbe der aktiven Zeilen-/Spaltenüberschrift fest. |
| [getActiveSheet()](#getActiveSheet--) | Ermittelt das aktive Blatt |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Ermittelt den Index des aktiven Blatts. |
| [getActiveTabStyle()](#getActiveTabStyle--) | Legt den Stil des aktiven Tabs fest. |
| [getAutoRefreshChart()](#getAutoRefreshChart--) | Ermittelt, ob das Diagrammbild beim Aktualisieren des Zellenwerts aktualisiert wird. Der Standardwert ist true. |
| [getBackColor()](#getBackColor--) | Ruft die Hintergrundfarbe im WebControl ab |
| [getBorderColor()](#getBorderColor--) | Ruft die Rahmenfarbe im WebControl ab |
| [getBorderStyle()](#getBorderStyle--) | Ruft den Rahmenstil im WebControl ab |
| [getBorderWidth()](#getBorderWidth--) | Ruft die Rahmenbreite im WebControl ab |
| [getBottomTableStyle()](#getBottomTableStyle--) | Ermittelt den Stil der unteren Leiste der Steuerung. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Ruft die CssClass im WebControl ab |
| [getCurrentPageIndex()](#getCurrentPageIndex--) | Ermittelt den aktuellen Seitenindex im Paging-Modus. |
| [getCustomCalculationEngine()](#getCustomCalculationEngine--) | Stellt die benutzerdefinierte Berechnungs‑Engine des Benutzers dar, um die Standard‑Berechnungs‑Engine von Aspose.Cells zu erweitern. |
| [getCustomCommandButtons()](#getCustomCommandButtons--) | Ermittelt die benutzerdefinierte Sammlung von Befehls-Schaltflächen |
| [getCustomStyleFileName()](#getCustomStyleFileName--) | Ermittelt den Dateinamen des benutzerdefinierten Stils. |
| [getDPI()](#getDPI--) | Ermittelt / legt die DPI des Geräts fest. |
| [getDefaultFontName()](#getDefaultFontName--) | Liefert den Standard-Schriftartnamen der Steuerung. |
| [getDefaultFontSize()](#getDefaultFontSize--) | Ermittelt die Standard-Schriftgröße der Steuerung. |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) | Ermittelt die Farbe der Standardgitterlinien. |
| [getDisplayCellTip()](#getDisplayCellTip--) | Ermittelt, ob Tipps angezeigt werden. Der Standardwert ist true. |
| [getEditMode()](#getEditMode--) | Ermittelt den Bearbeitungsmodus der Steuerung. |
| [getEnableAJAX()](#getEnableAJAX--) | Ermittelt, ob ein AJAX-Aufruf verwendet wird. Der Standardwert ist true. |
| [getEnableAsync()](#getEnableAsync--) | Ermittelt, ob Zellen-Daten asynchron geladen werden; empfohlen für ein Blatt mit mehr als 10.000 Zellen. |
| [getEnableClientColumnOperations()](#getEnableClientColumnOperations--) | Ermittelt, ob clientseitige Spaltenoperationen aktiviert werden. |
| [getEnableClientFreeze()](#getEnableClientFreeze--) | Ermittelt, ob clientseitige Freeze-Operationen aktiviert werden. |
| [getEnableClientMergeOperations()](#getEnableClientMergeOperations--) | Ermittelt, ob clientseitige Merge-Operationen aktiviert werden. |
| [getEnableClientResizeColumnRow()](#getEnableClientResizeColumnRow--) | Ermittelt, ob das clientseitige Ändern von Spalten und Zeilen aktiviert ist. |
| [getEnableClientRowOperations()](#getEnableClientRowOperations--) | Ermittelt, ob die clientseitigen Zeilenoperationen aktiviert sind. |
| [getEnableDoubleClickEvent()](#getEnableDoubleClickEvent--) | Ermittelt, ob das kundenseitige Doppelklick-Ereignis aktiviert ist. |
| [getEnableMetalLightEffect()](#getEnableMetalLightEffect--) | Ermittelt, ob der Metal-Lichteffekt angewendet wird. |
| [getEnablePaging()](#getEnablePaging--) | Ermittelt, ob der Paging-Modus der Steuerung aktiviert ist. |
| [getEnableStyleDialogbox()](#getEnableStyleDialogbox--) | Ermittelt, ob das clientseitige Stil-Dialogfeld aktiviert ist. |
| [getEnabled()](#getEnabled--) | Ruft den Aktivierungsstatus im WebControl ab |
| [getFilteredPaging()](#getFilteredPaging--) | Ermittelt, ob das Paging nach Datenfilterung aktiviert wird; wirkt nur, wenn EnablePaging true ist. |
| [getFont()](#getFont--) | Ruft die Schriftart im WebControl ab |
| [getForceValidation()](#getForceValidation--) | Ermittelt, ob die kundenseitige Validierung erzwungen wird. |
| [getForeColor()](#getForeColor--) | Ruft die Vordergrundfarbe im WebControl ab |
| [getFrameTableStyle()](#getFrameTableStyle--) | Ermittelt den Rahmenstil der Steuerung. |
| [getGoonDefaultSaveOperation()](#getGoonDefaultSaveOperation--) | Ermittelt, ob GridWeb die Standard‑Speicheroperation ausführt, der Standardwert ist true. |
| [getHeaderBarHeight()](#getHeaderBarHeight--) | Ermittelt die Höhe (System.Web.UI.WebControl.Unit) der oberen Kopfzeile der Steuerung. |
| [getHeaderBarStyle()](#getHeaderBarStyle--) | Ermittelt den Stil der Kopfzeile. |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) | Ermittelt den Stil der Kopfzeile der Steuerung. |
| [getHeaderBarWidth()](#getHeaderBarWidth--) | Ermittelt die Breite (System.Web.UI.WebControl.Unit) der linken Kopfzeile der Steuerung. |
| [getHeight()](#getHeight--) | Ermittelt die Höhe (System.Web.UI.WebControl.Unit) der Steuerung. |
| [getIgnoreStyleWithNoData()](#getIgnoreStyleWithNoData--) | Ermittelt, ob GridWeb das Anzeigen von Zeilen oder Spalten, die keine Zellwerte enthalten, aber dennoch formatiert sind, ignoriert. |
| [getLoadOptions()](#getLoadOptions--) | Stellt die Ladeoptionen für GridWeb dar. |
| [getMaxColumn()](#getMaxColumn--) | Ermittelt den maximalen Anzeigespaltenindex (nullbasiert) des Webblatts. |
| [getMaxRow()](#getMaxRow--) | Ermittelt den maximalen Anzeigereihenindex (nullbasiert) des Webblatts. |
| [getMessage()](#getMessage--) | Ermittelt die Meldung für das Raster. |
| [getMinColumn()](#getMinColumn--) | Ermittelt den minimalen Anzeigespaltenindex (nullbasiert) des Webblatts. |
| [getMinRow()](#getMinRow--) | Ermittelt den minimalen Anzeigereihenindex (nullbasiert) des Webblatts. |
| [getModifiedCells()](#getModifiedCells--) | Ermittelt die Sammlung der vom Client modifizierten Zellen. |
| [getNeedRenderGroupRows()](#getNeedRenderGroupRows--) | Ermittelt, ob Gruppenzeilen angezeigt werden. |
| [getNoHScroll()](#getNoHScroll--) | Ermittelt einen Wert, der angibt, ob die horizontale Bildlaufleiste ausgeblendet ist. |
| [getNoScroll()](#getNoScroll--) | Ermittelt, ob die Bildlaufleiste angezeigt werden soll. |
| [getNoVScroll()](#getNoVScroll--) | Ermittelt einen Wert, der angibt, ob die vertikale Bildlaufleiste ausgeblendet ist. |
| [getOnAjaxCallFinishedClientFunction()](#getOnAjaxCallFinishedClientFunction--) | Ermittelt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn der Ajax-Aufruf beendet ist. |
| [getOnCellErrorClientFunction()](#getOnCellErrorClientFunction--) | Ermittelt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn die Validierung einer Zelle fehlgeschlagen ist. |
| [getOnCellSelectedAjaxCallBackClientFunction()](#getOnCellSelectedAjaxCallBackClientFunction--) | Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Zelle ausgewählt wird. |
| [getOnCellSelectedClientFunction()](#getOnCellSelectedClientFunction--) | Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Zelle ausgewählt wird. |
| [getOnCellUnselectedClientFunction()](#getOnCellUnselectedClientFunction--) | Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Zelle deselektiert wird. |
| [getOnCellUpdatedClientFunction()](#getOnCellUpdatedClientFunction--) | Ermittelt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn der Wert einer Zelle aktualisiert wird. |
| [getOnContextMenuShowClientFunction()](#getOnContextMenuShowClientFunction--) | Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn das Kontextmenü angezeigt wird. |
| [getOnDoubleClickCellClientFunction()](#getOnDoubleClickCellClientFunction--) | Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Zelle doppelt angeklickt wird. |
| [getOnDoubleClickRowClientFunction()](#getOnDoubleClickRowClientFunction--) | Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Zeile doppelt angeklickt wird. |
| [getOnGridInitClientFunction()](#getOnGridInitClientFunction--) | Ermittelt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn das Raster initialisiert wird. |
| [getOnPageChangeClientFunction()](#getOnPageChangeClientFunction--) | Ermittelt die clientseitige Funktion, die nach dem Ändern des Seitenindex aufgerufen wird. Wirkt nur, wenn EnablePaging true ist. |
| [getOnPageSubmitClientFunction()](#getOnPageSubmitClientFunction--) | Ermittelt die clientseitige Funktion, die aufgerufen wird, bevor die Seite clientseitig übermittelt wird. |
| [getOnShapeSelectedClientFunction()](#getOnShapeSelectedClientFunction--) | Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Form ausgewählt wird. |
| [getOnSubmitClientFunction()](#getOnSubmitClientFunction--) | Ermittelt die clientseitige Funktion, die aufgerufen wird, bevor das Steuerelement clientseitig übermittelt wird. |
| [getOnlyAuto()](#getOnlyAuto--) | Ermittelt, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist; der Standardwert ist false. |
| [getPageSize()](#getPageSize--) | Ermittelt die Seitengröße im Paging-Modus. |
| [getPictureCachePath()](#getPictureCachePath--) | Ermittelt den Bildspeicherpfad für die Arbeitsmappe; alle Formen und Bilder werden in diesem Verzeichnis gespeichert. Der Standardpfad ist acwcache im Basisverzeichnis der aktuellen Anwendung. Benutzer müssen einen geplanten Dienst implementieren, um Dateien zu bereinigen, die die Sitzungszeit überschritten haben. |
| [getPresetStyle()](#getPresetStyle--) | Ermittelt den voreingestellten Stil. |
| [getRefreshValidation()](#getRefreshValidation--) | Ermittelt, ob der Validierungswert nach einer Zellwertänderung aktualisiert werden soll. |
| [getRenderHiddenRow()](#getRenderHiddenRow--) | Ermittelt, ob die ausgeblendete Zeile im GridControl gerendert wird; der Standardwert ist false. |
| [getRowHeightForCSV()](#getRowHeightForCSV--) | Ermittelt den Zeilenhöhenwert in Punkt für CSV-Dateien; der Standardwert ist 14,5. |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) | Gibt die Farbe der Pfeiltaste der Bildlaufleiste an. |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) | Gibt die Farbe der Bildlaufleiste des Steuerelements an. |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | Gibt die Hintergrundfarbe der ausgewählten Zellen im Mehrfachauswahlbereich an. |
| [getSelectCellColor()](#getSelectCellColor--) | Gibt die Farbe der ausgewählten Zellen im Mehrfachauswahlbereich an. |
| [getSelectCells()](#getSelectCells--) | Ruft die Sammlung der ausgewählten Zellen ab. |
| [getSessionStorePath()](#getSessionStorePath--) | Ruft den Pfad des Session-Cache-Speichers ab, wenn der Sitzungsmodus File oder ViewState usw. ist: gridweb.SessionStorePath="c:/mytempdir/session"; dann werden Sitzungsdaten in c:/mytempdir/session gespeichert. |
| [getSettings()](#getSettings--) | Stellt die Arbeitsmappeneinstellungen dar. |
| [getShowAddButton()](#getShowAddButton--) | Ermittelt, ob die Schaltfläche zum Hinzufügen eines Arbeitsblatts angezeigt wird. |
| [getShowBottomBar()](#getShowBottomBar--) | Gibt an, ob die Befehlsleiste (einschließlich Befehlsleiste und Registerkartenleiste) am unteren Rand des Steuerelements angezeigt wird. |
| [getShowCellEditBox()](#getShowCellEditBox--) | Ob Gridweb die Symbolleiste für das Bearbeitungsfeld wie in MS-EXCEL anzeigt. Wenn aktiviert, wird ein Bearbeitungsfeld für die aktuelle Zelle in Gridweb angezeigt. |
| [getShowCommandBarAtTop()](#getShowCommandBarAtTop--) | Gibt an, ob die Befehlsleiste (einschließlich Befehlsleiste und Registerkartenleiste) am oberen Rand des Steuerelements angezeigt wird. |
| [getShowContextMenu()](#getShowContextMenu--) | Ermittelt, ob das Kontextmenü angezeigt wird. Der Standardwert ist true. |
| [getShowDefaultGridLine()](#getShowDefaultGridLine--) | Ermittelt, ob die Standardgitternetzlinien der Zellen angezeigt werden. |
| [getShowHeaderBar()](#getShowHeaderBar--) | Ermittelt, ob die Kopfzeilenleiste angezeigt wird |
| [getShowLoading()](#getShowLoading--) | Gibt an, ob während des Postbacks zum Server ein Lade-Dialogfeld angezeigt wird. |
| [getShowLoadingPosition()](#getShowLoadingPosition--) | Gibt die linke, obere Position (in px) an, um das Lade-Dialogfeld während des Postbacks zum Server anzuzeigen usw. 100,200 bedeutet, dass die linke, obere Position des Lade-Dialogfelds bei 100px,200px liegt. |
| [getShowSaveButton()](#getShowSaveButton--) | Ermittelt, ob die Schaltfläche zum Speichern angezeigt wird. |
| [getShowSubmitButton()](#getShowSubmitButton--) | Ermittelt, ob die Schaltfläche zum Absenden angezeigt wird. |
| [getShowTabBar()](#getShowTabBar--) | Ermittelt, ob die Registerkartenleiste angezeigt wird. |
| [getShowTabNavigation()](#getShowTabNavigation--) | Ermittelt, ob die Registerkarten-Navigationsschaltfläche angezeigt wird, der Standardwert ist true. |
| [getShowUndoButton()](#getShowUndoButton--) | Ermittelt, ob die Rückgängig-Schaltfläche angezeigt wird. |
| [getSpanWrap()](#getSpanWrap--) | Gibt an, ob der Inhalt im Zellenbereich umgebrochen wird. Der Standardwert ist true. |
| [getTabIndex()](#getTabIndex--) | Ruft den TabIndex im WebControl ab |
| [getTabStyle()](#getTabStyle--) | Ermittelt den Stil der Registerkartenleiste. |
| [getToolTip()](#getToolTip--) | Ruft den ToolTip im WebControl ab |
| [getUseClientPageHeight()](#getUseClientPageHeight--) | Ermittelt, ob Gridweb die Höhe der Client-Seite als Steuerelementhöhe verwendet, geeignet, wenn Height="100%" gesetzt ist, Standardwert ist false. |
| [getVersion()](#getVersion--) | Ermittelt die Release‑Version. |
| [getViewPanelScrollLeft()](#getViewPanelScrollLeft--) | Ermittelt die Position der Bildlaufleiste des Ansichtsbereichs des Rasters. |
| [getViewPanelScrollTop()](#getViewPanelScrollTop--) | Ermittelt die Position der Bildlaufleiste des Ansichtsbereichs des Rasters. |
| [getViewTableStyle()](#getViewTableStyle--) | Ermittelt den Stil des Datenansichtsbereichs. |
| [getWidth()](#getWidth--) | Ermittelt die Breite (System.Web.UI.WebControl.Unit) des Steuerelements. |
| [getWorkSheets()](#getWorkSheets--) | Ermittelt die Sammlung der Arbeitsblätter. |
| [getXhtmlMode()](#getXhtmlMode--) | Ermittelt, ob der XHTML-Stil verwendet wird, der Standardwert ist true. |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream stream)](#importExcelFile-java.io.InputStream-) | Importiert aus einem Excel-Datei-Stream, einschließlich Festplattendatei-Stream oder Speicher-Stream. |
| [importExcelFile(InputStream stream, String passwordtoOpen)](#importExcelFile-java.io.InputStream-java.lang.String-) | Importiert aus einem Excel-Datei-Stream, einschließlich Festplattendatei-Stream oder Speicher-Stream. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Importiert aus einer Excel-Datei. |
| [importExcelFile(String fileName, String passwordtoOpen)](#importExcelFile-java.lang.String-java.lang.String-) | Importiert aus einer Excel-Datei. |
| [isCalculateFormula()](#isCalculateFormula--) | Ermittelt, ob Formeln nach Änderungen des Zellenwerts oder nach dem Import der Datei berechnet werden sollen. |
| [loadCSVFile(InputStream stream)](#loadCSVFile-java.io.InputStream-) | Lädt Daten aus einem CSV-Datei-Stream. |
| [loadCSVFile(String fileName)](#loadCSVFile-java.lang.String-) | Lädt Daten aus einer CSV-Datei. |
| [loadHTMLFile(InputStream stream)](#loadHTMLFile-java.io.InputStream-) | Lädt Daten aus einem HTML-Datei-Stream. |
| [loadHTMLFile(String fileName)](#loadHTMLFile-java.lang.String-) | Lädt Daten aus einer HTML-Datei. |
| [loadSpreadSheetMLFile(InputStream stream)](#loadSpreadSheetMLFile-java.io.InputStream-) | Lädt Daten aus einem SpreadSheetML-Datei-Stream. |
| [loadSpreadSheetMLFile(String fileName)](#loadSpreadSheetMLFile-java.lang.String-) | Lädt Daten aus einer SpreadSheetML-Datei. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshChartShape()](#refreshChartShape--) | Aktualisiert alle Diagrammbilder für das aktive Arbeitsblatt. |
| [saveCSVFile(OutputStream stream)](#saveCSVFile-java.io.OutputStream-) | Speichert Daten in einen CSV-Datei-Stream. |
| [saveCSVFile(String targetFile)](#saveCSVFile-java.lang.String-) | Speichert Daten in einer CSV-Datei. |
| [saveCustomStyleFile(String fileName)](#saveCustomStyleFile-java.lang.String-) | Speichert die aktuellen Stil-Daten der Steuerung in einer XML-Datei. |
| [saveHTMLFile(OutputStream stream)](#saveHTMLFile-java.io.OutputStream-) | Speichert Daten in einen HTML-Datei-Stream. |
| [saveHTMLFile(String targetFile)](#saveHTMLFile-java.lang.String-) | Speichert Daten in einer HTML-Datei. |
| [saveSpreadSheetMLFile(OutputStream stream)](#saveSpreadSheetMLFile-java.io.OutputStream-) | Speichert Daten in einen SpreadSheetML-Datei-Stream. |
| [saveSpreadSheetMLFile(String targetFile)](#saveSpreadSheetMLFile-java.lang.String-) | Speichert Daten in einer SpreadSheetML-Datei. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)](#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [saveToExcelFile(OutputStream stream, int format)](#saveToExcelFile-java.io.OutputStream-int-) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [saveToExcelFile(String targetFile)](#saveToExcelFile-java.lang.String-) | Speichert die Arbeitsblätter in einer Excel-Datei im Excel‑2003‑Format. |
| [saveToExcelFile(String targetFile, GridSaveOptions saveOptions)](#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [saveToExcelFile(String targetFile, int format)](#saveToExcelFile-java.lang.String-int-) | Speichert die Arbeitsblätter in einer Excel-Datei. |
| [setACWClientPath(String value)](#setACWClientPath-java.lang.String-) | Legt den Webpfad der Skript-/Bilddateien der Steuerung fest. |
| [setACWLanguageFileUrl(String value)](#setACWLanguageFileUrl-java.lang.String-) | Legt die Web‑URL der Sprachdatei der Steuerung fest. |
| [setActiveCell(GridCell value)](#setActiveCell-com.aspose.gridweb.GridCell-) | Legt die aktive Zelle des aktuellen Blatts fest. |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | Legt die Hintergrundfarbe der aktiven Zelle fest. |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | Legt die Farbe der aktiven Zelle fest. |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | Legt die Hintergrundfarbe der aktiven Zeilen-/Spaltenüberschrift fest. |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | Legt die Farbe der aktiven Zeilen-/Spaltenüberschrift fest. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Legt den Index des aktiven Blatts fest. |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Legt den Stil des aktiven Tabs fest. |
| [setAutoRefreshChart(boolean value)](#setAutoRefreshChart-boolean-) | Legt fest, ob das Diagrammbild beim Aktualisieren des Zellenwerts aktualisiert wird. Der Standardwert ist true. |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Legt die Hintergrundfarbe im WebControl fest |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Legt die Rahmenfarbe im WebControl fest |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Legt den Rahmenstil im WebControl fest |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Legt die Rahmenbreite im WebControl fest |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) | Legt den Stil der unteren Leiste der Steuerung fest. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Legt fest, ob die Formel nach Änderungen des Zellenwerts oder nach dem Import einer Datei berechnet wird. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Setzt die CssClass im WebControl |
| [setCurrentPageIndex(int value)](#setCurrentPageIndex-int-) | Legt den aktuellen Seitenindex im Paging-Modus fest. |
| [setCustomCalculationEngine(GridAbstractCalculationEngine value)](#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-) | Stellt die benutzerdefinierte Berechnungs‑Engine des Benutzers dar, um die Standard‑Berechnungs‑Engine von Aspose.Cells zu erweitern. |
| [setCustomStyle(InputStream stream)](#setCustomStyle-java.io.InputStream-) | Legt die benutzerdefinierte Stildatei aus einem Stream fest, einschließlich Dateistream von der Festplatte oder Speicherstream. |
| [setCustomStyleFileName(String value)](#setCustomStyleFileName-java.lang.String-) | Legt den Namen der benutzerdefinierten Stildatei fest. |
| [setDPI(double value)](#setDPI-double-) | Ermittelt / legt die DPI des Geräts fest. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Legt den Standard‑Schriftartnamen des Steuerelements fest. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | Legt die Standard-Schriftgröße der Steuerung fest. |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) | Legt die Standardfarbe der Rasterlinien fest. |
| [setDisplayCellTip(boolean value)](#setDisplayCellTip-boolean-) | Legt fest, ob Tipps angezeigt werden. Der Standardwert ist true. |
| [setEditMode(boolean value)](#setEditMode-boolean-) | Legt den Bearbeitungsmodus der Steuerung fest. |
| [setEnableAJAX(boolean value)](#setEnableAJAX-boolean-) | Legt fest, ob ein AJAX-Aufruf verwendet wird. Der Standardwert ist true. |
| [setEnableAsync(boolean value)](#setEnableAsync-boolean-) | Legt fest, ob Zellen-Daten asynchron geladen werden; empfohlen für ein Blatt mit mehr als 10.000 Zellen. |
| [setEnableClientColumnOperations(boolean value)](#setEnableClientColumnOperations-boolean-) | Legt fest, ob clientseitige Spaltenoperationen aktiviert werden. |
| [setEnableClientFreeze(boolean value)](#setEnableClientFreeze-boolean-) | Legt fest, ob clientseitige Freeze-Operationen aktiviert werden. |
| [setEnableClientMergeOperations(boolean value)](#setEnableClientMergeOperations-boolean-) | Legt fest, ob clientseitige Merge-Operationen aktiviert werden. |
| [setEnableClientResizeColumnRow(boolean value)](#setEnableClientResizeColumnRow-boolean-) | Legt fest, ob das clientseitige Ändern der Größe von Spalten und Zeilen aktiviert wird. |
| [setEnableClientRowOperations(boolean value)](#setEnableClientRowOperations-boolean-) | Legt fest, ob clientseitige Zeilenoperationen aktiviert werden. |
| [setEnableDoubleClickEvent(boolean value)](#setEnableDoubleClickEvent-boolean-) | Legt fest, ob das kundenseitige Doppelklick-Ereignis aktiviert wird. |
| [setEnableMetalLightEffect(boolean value)](#setEnableMetalLightEffect-boolean-) | Legt fest, ob der Metal-Light-Effekt angewendet wird. |
| [setEnablePaging(boolean value)](#setEnablePaging-boolean-) | Legt fest, ob der Paging-Modus der Steuerung aktiviert wird. |
| [setEnableStyleDialogbox(boolean value)](#setEnableStyleDialogbox-boolean-) | Legt fest, ob das clientseitige Stil-Dialogfeld aktiviert wird. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Setzt das Enabled im WebControl |
| [setFilteredPaging(boolean value)](#setFilteredPaging-boolean-) | Legt fest, ob das Paging nach Datenfilterung aktiviert wird; wirkt nur, wenn EnablePaging true ist. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Legt den Schriftarten-Ordner fest |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Setzt die Schriftordner |
| [setForceValidation(boolean value)](#setForceValidation-boolean-) | Legt fest, ob die kundenseitige Validierung erzwungen wird. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Setzt die ForeColor im WebControl |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) | Legt den Rahmenstil der Steuerung fest. |
| [setGoonDefaultSaveOperation(boolean value)](#setGoonDefaultSaveOperation-boolean-) | Legt fest, ob GridWeb die Standard‑Speicheroperation ausführt, der Standardwert ist true. |
| [setHeaderBarHeight(Unit value)](#setHeaderBarHeight-com.aspose.gridweb.Unit-) | Legt die Höhe (System.Web.UI.WebControl.Unit) der oberen Kopfzeile der Steuerung fest. |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) | Legt den Stil der Kopfzeile fest. |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) | Legt den Stil der Kopfzeilenleiste des Steuerelements fest. |
| [setHeaderBarWidth(Unit value)](#setHeaderBarWidth-com.aspose.gridweb.Unit-) | Legt die Breite ( System.Web.UI.WebControl.Unit ) oder die linke Kopfzeilenleiste des Steuerelements fest. |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Legt die Höhe ( System.Web.UI.WebControl.Unit ) des Steuerelements fest. |
| [setIgnoreStyleWithNoData(boolean value)](#setIgnoreStyleWithNoData-boolean-) | Legt fest, ob GridWeb das Anzeigen von Zeilen oder Spalten ignoriert, die keine Zellwerte enthalten, aber dennoch formatiert sind. |
| [setLoadOptions(GridLoadOptions value)](#setLoadOptions-com.aspose.gridweb.GridLoadOptions-) | Stellt die Ladeoptionen für GridWeb dar. |
| [setMaxColumn(int value)](#setMaxColumn-int-) | Legt den maximalen Anzeigespaltenindex (nullbasiert) des Webblatts fest. |
| [setMaxRow(int value)](#setMaxRow-int-) | Legt den maximalen Anzeigereihenindex (nullbasiert) des Webblatts fest. |
| [setMessage(String value)](#setMessage-java.lang.String-) | Legt die Meldung für das Raster fest. |
| [setMinColumn(int value)](#setMinColumn-int-) | Legt den minimalen Anzeigespaltenindex (nullbasiert) des Webblatts fest. |
| [setMinRow(int value)](#setMinRow-int-) | Legt den minimalen Anzeigereihenindex (nullbasiert) des Webblatts fest. |
| [setNeedRenderGroupRows(boolean value)](#setNeedRenderGroupRows-boolean-) | Legt fest, ob Gruppenzeilen angezeigt werden. |
| [setNoHScroll(boolean value)](#setNoHScroll-boolean-) | Legt einen Wert fest, der angibt, ob die horizontale Bildlaufleiste ausgeblendet ist. |
| [setNoScroll(boolean value)](#setNoScroll-boolean-) | Legt fest, ob die Bildlaufleiste angezeigt wird. |
| [setNoVScroll(boolean value)](#setNoVScroll-boolean-) | Legt einen Wert fest, der angibt, ob die vertikale Bildlaufleiste ausgeblendet ist. |
| [setOnAjaxCallFinishedClientFunction(String value)](#setOnAjaxCallFinishedClientFunction-java.lang.String-) | Legt den Namen der clientseitigen Funktion fest, die aufgerufen wird, wenn der Ajax-Aufruf abgeschlossen ist. |
| [setOnCellErrorClientFunction(String value)](#setOnCellErrorClientFunction-java.lang.String-) | Legt den Namen der clientseitigen Funktion fest, die aufgerufen wird, wenn die Validierung einer Zelle fehlschlägt. |
| [setOnCellSelectedAjaxCallBackClientFunction(String value)](#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-) | Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zelle ausgewählt wird. |
| [setOnCellSelectedClientFunction(String value)](#setOnCellSelectedClientFunction-java.lang.String-) | Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zelle ausgewählt wird. |
| [setOnCellUnselectedClientFunction(String value)](#setOnCellUnselectedClientFunction-java.lang.String-) | Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zelle deselektiert wird. |
| [setOnCellUpdatedClientFunction(String value)](#setOnCellUpdatedClientFunction-java.lang.String-) | Legt den Namen der clientseitigen Funktion fest, die aufgerufen wird, wenn der Wert einer Zelle aktualisiert wird. |
| [setOnContextMenuShowClientFunction(String value)](#setOnContextMenuShowClientFunction-java.lang.String-) | Legt die clientseitige Funktion fest, die aufgerufen wird, wenn das Kontextmenü angezeigt wird. |
| [setOnDoubleClickCellClientFunction(String value)](#setOnDoubleClickCellClientFunction-java.lang.String-) | Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zelle doppelt angeklickt wird. |
| [setOnDoubleClickRowClientFunction(String value)](#setOnDoubleClickRowClientFunction-java.lang.String-) | Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zeile doppelt angeklickt wird. |
| [setOnGridInitClientFunction(String value)](#setOnGridInitClientFunction-java.lang.String-) | Legt den Namen der clientseitigen Funktion fest, die aufgerufen wird, wenn das Raster initialisiert wird. |
| [setOnPageChangeClientFunction(String value)](#setOnPageChangeClientFunction-java.lang.String-) | Legt die clientseitige Funktion fest, die nach dem Ändern des Seitenindex aufgerufen wird. Wirkt nur, wenn EnablePaging true ist. |
| [setOnPageSubmitClientFunction(String value)](#setOnPageSubmitClientFunction-java.lang.String-) | Legt die clientseitige Funktion fest, die aufgerufen wird, bevor die Seite clientseitig übermittelt wird. |
| [setOnShapeSelectedClientFunction(String value)](#setOnShapeSelectedClientFunction-java.lang.String-) | Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Form ausgewählt wird. |
| [setOnSubmitClientFunction(String value)](#setOnSubmitClientFunction-java.lang.String-) | Legt die Client-Funktion fest, die vor dem Absenden der Steuerung auf der Clientseite aufgerufen wird. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Legt fest, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist; der Standardwert ist false. |
| [setPageSize(int value)](#setPageSize-int-) | Legt die Seitengröße im Paging-Modus fest. |
| [setPictureCachePath(String value)](#setPictureCachePath-java.lang.String-) | Legt den Bildspeicherpfad für die Arbeitsmappe fest, alle Formen und Bilder werden in diesem Verzeichnis gespeichert; der Standardpfad ist acwcache im Basisverzeichnis der aktuellen Anwendung. Benutzer müssen einen geplanten Dienst implementieren, um Dateien zu bereinigen, die die Sitzungszeit überschritten haben. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Legt den voreingestellten Stil fest. |
| [setRefreshValidation(boolean value)](#setRefreshValidation-boolean-) | Legt fest, ob der Validierungswert nach Änderungen des Zellenwerts aktualisiert wird. |
| [setRenderHiddenRow(boolean value)](#setRenderHiddenRow-boolean-) | Legt fest, ob die ausgeblendete Zeile im GridControl gerendert wird; der Standardwert ist false. |
| [setRowHeightForCSV(double value)](#setRowHeightForCSV-double-) | Legt den Zeilenhöhenwert in Punkt für CSV-Dateien fest, Standardwert ist 14,5. |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) | Gibt die Farbe der Pfeiltaste der Bildlaufleiste an. |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) | Gibt die Farbe der Bildlaufleiste des Steuerelements an. |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | Gibt die Hintergrundfarbe der ausgewählten Zellen im Mehrfachauswahlbereich an. |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | Gibt die Farbe der ausgewählten Zellen im Mehrfachauswahlbereich an. |
| [setSessionStorePath(String value)](#setSessionStorePath-java.lang.String-) | Legt den Pfad für den Sitzungs-Cache fest, wenn der Sitzungsmodus File oder ViewState ist usw.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; anschließend werden Sitzungsdaten in c:/mytempdir/session gespeichert. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridweb.GridWorkbookSettings-) | Stellt die Arbeitsmappeneinstellungen dar. |
| [setShowAddButton(boolean value)](#setShowAddButton-boolean-) | Legt fest, ob die Schaltfläche zum Hinzufügen eines Arbeitsblatts angezeigt wird. |
| [setShowBottomBar(boolean value)](#setShowBottomBar-boolean-) | Gibt an, ob die Befehlsleiste (einschließlich Befehlsleiste und Registerkartenleiste) am unteren Rand des Steuerelements angezeigt wird. |
| [setShowCellEditBox(boolean value)](#setShowCellEditBox-boolean-) | Ob Gridweb die Symbolleiste für das Bearbeitungsfeld wie in MS-EXCEL anzeigt. Wenn aktiviert, wird ein Bearbeitungsfeld für die aktuelle Zelle in Gridweb angezeigt. |
| [setShowCommandBarAtTop(boolean value)](#setShowCommandBarAtTop-boolean-) | Gibt an, ob die Befehlsleiste (einschließlich Befehlsleiste und Registerkartenleiste) am oberen Rand des Steuerelements angezeigt wird. |
| [setShowContextMenu(boolean value)](#setShowContextMenu-boolean-) | Legt fest, ob das Kontextmenü angezeigt wird. Der Standardwert ist true. |
| [setShowDefaultGridLine(boolean value)](#setShowDefaultGridLine-boolean-) | Legt fest, ob die Standardgitterlinien der Zellen angezeigt werden. |
| [setShowHeaderBar(boolean value)](#setShowHeaderBar-boolean-) | Legt fest, ob die Header-Leiste angezeigt wird |
| [setShowLoading(boolean value)](#setShowLoading-boolean-) | Gibt an, ob während des Postbacks zum Server ein Lade-Dialogfeld angezeigt wird. |
| [setShowLoadingPosition(String value)](#setShowLoadingPosition-java.lang.String-) | Gibt die linke, obere Position (in px) an, um das Lade-Dialogfeld während des Postbacks zum Server anzuzeigen usw. 100,200 bedeutet, dass die linke, obere Position des Lade-Dialogfelds bei 100px,200px liegt. |
| [setShowSaveButton(boolean value)](#setShowSaveButton-boolean-) | Legt fest, ob die Schaltfläche zum Speichern angezeigt wird. |
| [setShowSubmitButton(boolean value)](#setShowSubmitButton-boolean-) | Legt fest, ob die Schaltfläche zum Absenden angezeigt wird. |
| [setShowTabBar(boolean value)](#setShowTabBar-boolean-) | Legt fest, ob die Registerkartenleiste angezeigt wird. |
| [setShowTabNavigation(boolean value)](#setShowTabNavigation-boolean-) | Legt fest, ob die Registerkarten-Navigationsschaltfläche angezeigt wird; der Standardwert ist true. |
| [setShowUndoButton(boolean value)](#setShowUndoButton-boolean-) | Legt fest, ob die Rückgängig-Schaltfläche angezeigt wird. |
| [setSpanWrap(boolean value)](#setSpanWrap-boolean-) | Gibt an, ob der Inhalt im Zellenbereich umgebrochen wird. Der Standardwert ist true. |
| [setTabIndex(short value)](#setTabIndex-short-) | Setzt den TabIndex im WebControl |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Legt den Stil der Registerkartenleiste fest. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Setzt den ToolTip im WebControl |
| [setUseClientPageHeight(boolean value)](#setUseClientPageHeight-boolean-) | Legt fest, ob GridWeb die Höhe der Clientseite als Steuerungshöhe verwendet, geeignet für die Einstellung Height=\"100%\"; der Standardwert ist false. |
| [setViewPanelScrollLeft(String value)](#setViewPanelScrollLeft-java.lang.String-) | Legt die Position der Bildlaufleiste des Ansichtsbereichs des Rasters fest. |
| [setViewPanelScrollTop(String value)](#setViewPanelScrollTop-java.lang.String-) | Legt die Position der Bildlaufleiste des Ansichtsbereichs des Rasters fest. |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) | Legt den Stil des Datenansichtsbereichs fest. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Legt die Breite (System.Web.UI.WebControl.Unit) der Steuerung fest. |
| [setXhtmlMode(boolean value)](#setXhtmlMode-boolean-) | Legt fest, ob der XHTML-Stil verwendet wird; der Standardwert ist true. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWeb() {#GridWeb--}
```
public GridWeb()
```


### AfterColumnFilter {#AfterColumnFilter}
```
public RowColumnEventHandler AfterColumnFilter
```


Tritt auf, nachdem die Spalte gefiltert wurde.

### AjaxCallFinished {#AjaxCallFinished}
```
public WorkbookEventHandler AjaxCallFinished
```


Wird ausgelöst, wenn das AJAX-Update der Steuerung abgeschlossen ist. (EnableAJAX muss auf true gesetzt sein)

### BeforeColumnFilter {#BeforeColumnFilter}
```
public RowColumnEventHandler BeforeColumnFilter
```


Tritt auf, bevor die Spalte gefiltert wird.

### CellClickOnAjax {#CellClickOnAjax}
```
public CellEventStringHandler CellClickOnAjax
```


Tritt auf, wenn die Zelle angeklickt wird, und erfordert einen Ajax-Callback für dieses Ereignis.

### CellClientUpdate {#CellClientUpdate}
```
public CellEventHandler CellClientUpdate
```


Tritt auf, wenn ein Client‑Zellen‑Update erfolgt. Wenn dieses Ereignis ausgelöst wird, enthält sein Parameter e.Argument den Namen des Befehls.

### CellCommand {#CellCommand}
```
public CellEventHandler CellCommand
```


Tritt auf, wenn der Befehls‑Hyperlink einer Zelle angeklickt wird. Wenn dieses Ereignis ausgelöst wird, enthält sein Parameter e.Argument den Namen des Befehls.

### CellDoubleClick {#CellDoubleClick}
```
public CellEventHandler CellDoubleClick
```


Tritt auf, wenn die Zelle doppelt angeklickt wird.

### CellModifiedOnAjax {#CellModifiedOnAjax}
```
public CellEventHandler CellModifiedOnAjax
```


Tritt auf, wenn die Zelle in einem Ajax-Aufruf geändert wird.

### ColumnDeleted {#ColumnDeleted}
```
public RowColumnEventHandler ColumnDeleted
```


Tritt auf, wenn ein Benutzer eine Spalte über das clientseitige Menü löscht.

### ColumnDeleting {#ColumnDeleting}
```
public RowColumnEventHandler ColumnDeleting
```


Tritt auf, wenn ein Benutzer versucht, eine Spalte über das clientseitige Menü zu löschen. Sie können dieses Ereignis behandeln und den Parameter cancel auf True setzen, um den Löschvorgang abzubrechen.

### ColumnDoubleClick {#ColumnDoubleClick}
```
public RowColumnEventHandler ColumnDoubleClick
```


Tritt auf, wenn die Spaltenüberschrift doppelt angeklickt wird.

### ColumnInserted {#ColumnInserted}
```
public RowColumnEventHandler ColumnInserted
```


Tritt auf, wenn ein Benutzer eine Spalte über das clientseitige Menü einfügt.

### CustomCommand {#CustomCommand}
```
public CustomCommandEventHandler CustomCommand
```


Tritt auf, wenn ein Benutzer eine benutzerdefinierte Befehls-Schaltfläche anklickt.

### LoadCustomData {#LoadCustomData}
```
public WorkbookEventHandler LoadCustomData
```


Wird ausgelöst, wenn der SessionMode des Steuerelements auf Custom gesetzt ist und Tabellendaten geladen werden müssen. Sie können dieses Ereignis im benutzerdefinierten Sitzungsmodus behandeln, um Tabellendaten aus einer Datei oder Datenbank zu laden.

### PageIndexChanged {#PageIndexChanged}
```
public WorkbookEventHandler PageIndexChanged
```


Tritt auf, wenn sich der Blattseitenindex der Steuerung ändert.

### RowDeleted {#RowDeleted}
```
public RowColumnEventHandler RowDeleted
```


Tritt auf, wenn ein Benutzer eine Zeile über das clientseitige Menü gelöscht hat.

### RowDeleting {#RowDeleting}
```
public RowColumnEventHandler RowDeleting
```


Tritt auf, wenn ein Benutzer versucht, eine Zeile über das clientseitige Menü zu löschen. Sie können dieses Ereignis behandeln und eine RejectDeleteException auslösen, um den Löschvorgang abzubrechen.

### RowDoubleClick {#RowDoubleClick}
```
public RowColumnEventHandler RowDoubleClick
```


Tritt auf, wenn die Zeilenüberschrift doppelt angeklickt wird.

### RowInserted {#RowInserted}
```
public RowColumnEventHandler RowInserted
```


Tritt auf, wenn ein Benutzer eine Zeile über das clientseitige Menü einfügt.

### SaveCommand {#SaveCommand}
```
public WorkbookEventHandler SaveCommand
```


Tritt auf, wenn die Schaltfläche "Speichern" angeklickt wird.

### SheetAdded {#SheetAdded}
```
public SheetEventHandler SheetAdded
```


Tritt auf, wenn ein Benutzer ein Arbeitsblatt über das Symbolleistenmenü hinzufügt.

### SheetTabClick {#SheetTabClick}
```
public WorkbookEventHandler SheetTabClick
```


Tritt auf, wenn das Blattregister angeklickt wird.

### SubmitCommand {#SubmitCommand}
```
public WorkbookEventHandler SubmitCommand
```


Tritt auf, wenn die Schaltfläche "Absenden" angeklickt wird.

### UndoCommand {#UndoCommand}
```
public WorkbookEventHandler UndoCommand
```


Tritt auf, wenn die Schaltfläche "Rückgängig" angeklickt wird.

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Berechnet das Ergebnis von Formeln.

### createChildControls() {#createChildControls--}
```
public void createChildControls()
```


Implementiert CreateChildControls von WebControl, nur intern verwendet.

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
### getACWClientPath() {#getACWClientPath--}
```
public String getACWClientPath()
```


Ermittelt den Web‑Pfad der Skript‑/Bilddateien des Steuerelements. Beispiel: "http://localhost/acw\_client". Sie können diesen Wert auch in der web.config‑Datei festlegen. Fügen Sie diesen Abschnitt zum `<configuration>`‑Abschnitt hinzu:
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Returns:**
java.lang.String
### getACWLanguageFileUrl() {#getACWLanguageFileUrl--}
```
public String getACWLanguageFileUrl()
```


Ermittelt die Web‑URL der Sprachdatei des Steuerelements. Beispiel: "/acw\_client/lang\_en.js".
Standardmäßig wird eine integrierte englische Datei verwendet.


**Returns:**
java.lang.String
### getActiveCell() {#getActiveCell--}
```
public GridCell getActiveCell()
```


Ermittelt die aktive Zelle des aktuellen Arbeitsblatts. Seit Version 1.9.0.1 ist sie schreibbar.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getActiveCellBgColor() {#getActiveCellBgColor--}
```
public Color getActiveCellBgColor()
```


Legt die Hintergrundfarbe der aktiven Zelle fest.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveCellColor() {#getActiveCellColor--}
```
public Color getActiveCellColor()
```


Legt die Farbe der aktiven Zelle fest.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderBgColor() {#getActiveHeaderBgColor--}
```
public Color getActiveHeaderBgColor()
```


Legt die Hintergrundfarbe der aktiven Zeilen-/Spaltenüberschrift fest.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderColor() {#getActiveHeaderColor--}
```
public Color getActiveHeaderColor()
```


Legt die Farbe der aktiven Zeilen-/Spaltenüberschrift fest.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveSheet() {#getActiveSheet--}
```
public GridWorksheet getActiveSheet()
```


Ermittelt das aktive Blatt

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Ermittelt den Index des aktiven Arbeitsblatts. Entspricht WebWorksheets.ActiveSheetIndex.

**Returns:**
int
### getActiveTabStyle() {#getActiveTabStyle--}
```
public GridTableItemStyle getActiveTabStyle()
```


Legt den Stil des aktiven Tabs fest.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getAutoRefreshChart() {#getAutoRefreshChart--}
```
public boolean getAutoRefreshChart()
```


Ermittelt, ob das Diagrammbild beim Aktualisieren des Zellenwerts aktualisiert wird. Der Standardwert ist true.

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Ruft die Hintergrundfarbe im WebControl ab

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Ruft die Rahmenfarbe im WebControl ab

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Ruft den Rahmenstil im WebControl ab

Siehe [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Ruft die Rahmenbreite im WebControl ab

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```


Ermittelt den Stil der unteren Leiste der Steuerung.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


Ruft die CssClass im WebControl ab

**Returns:**
java.lang.String
### getCurrentPageIndex() {#getCurrentPageIndex--}
```
public int getCurrentPageIndex()
```


Ermittelt den aktuellen Seitenindex im Paging-Modus.

**Remarks**

Im Paging‑Modus zeigt das Steuerelement einmal PageSize Zeilen Daten an und stellt das Seitenwahl‑Steuerelement in der Registerkartenleiste dar.

**Returns:**
int
### getCustomCalculationEngine() {#getCustomCalculationEngine--}
```
public GridAbstractCalculationEngine getCustomCalculationEngine()
```


Stellt die benutzerdefinierte Berechnungs‑Engine des Benutzers dar, um die Standard‑Berechnungs‑Engine von Aspose.Cells zu erweitern.

**Returns:**
[GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine)
### getCustomCommandButtons() {#getCustomCommandButtons--}
```
public CustomCommandButtonCollection getCustomCommandButtons()
```


Ermittelt die benutzerdefinierte Sammlung von Befehls-Schaltflächen

**Returns:**
[CustomCommandButtonCollection](../../com.aspose.gridweb/customcommandbuttoncollection)
### getCustomStyleFileName() {#getCustomStyleFileName--}
```
public String getCustomStyleFileName()
```


Ermittelt den Dateinamen des benutzerdefinierten Stils.

**Remarks**

Die benutzerdefinierte Stildatei ist eine XML-Datei. Wenn der Dateiname gesetzt wird, wird die Datei sofort geladen. Hier ist der Inhalt des "Standard-Voreinstellungsstils" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Example**

```
         		GridWeb1.setCustomStyleFileName("c:\\style\\mystyle.xml");
```

**Returns:**
java.lang.String
### getDPI() {#getDPI--}
```
public static double getDPI()
```


Ermittelt / legt die DPI des Geräts fest.

**Remarks**

**Returns:**
double
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Liefert den Standard-Schriftartnamen der Steuerung.

**Example**

```
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


Ermittelt die Standard-Schriftgröße der Steuerung.

**Example**

```
         		GridWeb1.setDefaultFontSize(new FontUnit("10pt"));
```

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getDefaultGridLineColor() {#getDefaultGridLineColor--}
```
public Color getDefaultGridLineColor()
```


Ermittelt die Farbe der Standardgitterlinien.

**Example**

```
         		GridWeb1.setDefaultGridLineColor(Color.getRed());
```

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getDisplayCellTip() {#getDisplayCellTip--}
```
public boolean getDisplayCellTip()
```


Ermittelt, ob Tipps angezeigt werden. Der Standardwert ist true.

**Returns:**
boolean
### getEditMode() {#getEditMode--}
```
public boolean getEditMode()
```


Ermittelt den Bearbeitungsmodus der Steuerung.

**Remarks**

Wenn auf true gesetzt, sind die Zellen der Steuerung editierbar, und das "save"- und das "undo"-Symbol werden angezeigt. Wenn auf false gesetzt, sind die Zellen der Steuerung schreibgeschützt, und das "save"- und das "undo"-Symbol werden nicht angezeigt.

**Returns:**
boolean
### getEnableAJAX() {#getEnableAJAX--}
```
public boolean getEnableAJAX()
```


Ermittelt, ob ein AJAX-Aufruf verwendet wird. Der Standardwert ist true.

**Returns:**
boolean
### getEnableAsync() {#getEnableAsync--}
```
public boolean getEnableAsync()
```


Ermittelt, ob Zellen-Daten asynchron geladen werden; empfohlen für ein Blatt mit mehr als 10.000 Zellen.

**Returns:**
boolean
### getEnableClientColumnOperations() {#getEnableClientColumnOperations--}
```
public boolean getEnableClientColumnOperations()
```


Ermittelt, ob clientseitige Spaltenoperationen aktiviert werden.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer das Kontextmenü verwenden, um Spalten hinzuzufügen/zu entfernen.

**Returns:**
boolean
### getEnableClientFreeze() {#getEnableClientFreeze--}
```
public boolean getEnableClientFreeze()
```


Ermittelt, ob clientseitige Freeze-Operationen aktiviert werden.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer das Kontextmenü verwenden, um Bereiche zu fixieren/zu lösen.

**Returns:**
boolean
### getEnableClientMergeOperations() {#getEnableClientMergeOperations--}
```
public boolean getEnableClientMergeOperations()
```


Ermittelt, ob clientseitige Merge-Operationen aktiviert werden.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer das Kontextmenü verwenden, um Zellen zu verbinden/zu trennen.

**Returns:**
boolean
### getEnableClientResizeColumnRow() {#getEnableClientResizeColumnRow--}
```
public boolean getEnableClientResizeColumnRow()
```


Ermittelt, ob das clientseitige Ändern von Spalten und Zeilen aktiviert ist.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer die Spalte und Zeile auf der Clientseite in der Größe anpassen.

**Returns:**
boolean
### getEnableClientRowOperations() {#getEnableClientRowOperations--}
```
public boolean getEnableClientRowOperations()
```


Ermittelt, ob die clientseitigen Zeilenoperationen aktiviert sind.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer das Kontextmenü verwenden, um Zeilen hinzuzufügen/zu entfernen.

**Returns:**
boolean
### getEnableDoubleClickEvent() {#getEnableDoubleClickEvent--}
```
public boolean getEnableDoubleClickEvent()
```


Ermittelt, ob das kundenseitige Doppelklick-Ereignis aktiviert ist.

**Remarks**

Wenn auf true gesetzt, empfängt die Steuerung clientseitige Doppelklick‑Ereignisse und Sie können diese Ereignisse auf der Serverseite verarbeiten. Andernfalls ignoriert die Steuerung alle Doppelklick‑Ereignisse.

**Returns:**
boolean
### getEnableMetalLightEffect() {#getEnableMetalLightEffect--}
```
public boolean getEnableMetalLightEffect()
```


Ermittelt, ob der Metal-Lichteffekt angewendet wird.

**Returns:**
boolean
### getEnablePaging() {#getEnablePaging--}
```
public boolean getEnablePaging()
```


Ermittelt, ob der Paging-Modus der Steuerung aktiviert ist.

**Remarks**

Wenn auf true gesetzt, zeigt die Steuerung einmal PageSize Zeilen Daten an und zeigt das Seiten‑Auswahl‑Steuerelement in der Tab‑Leiste an.

**Returns:**
boolean
### getEnableStyleDialogbox() {#getEnableStyleDialogbox--}
```
public boolean getEnableStyleDialogbox()
```


Ermittelt, ob das clientseitige Stil-Dialogfeld aktiviert ist.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer das Stil‑Dialogfeld verwenden, um den Stil einer Zelle festzulegen, indem er im Kontextmenü "Format Cell..." auswählt.

**Returns:**
boolean
### getEnabled() {#getEnabled--}
```
public boolean getEnabled()
```


Ruft den Aktivierungsstatus im WebControl ab

**Returns:**
boolean
### getFilteredPaging() {#getFilteredPaging--}
```
public boolean getFilteredPaging()
```


Ermittelt, ob das Paging nach Datenfilterung aktiviert wird; wirkt nur, wenn EnablePaging true ist.

**Remarks**

Wenn auf true gesetzt, paginiert die Steuerung basierend auf gefilterten Daten, der Standardwert ist false.

**Returns:**
boolean
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Ruft die Schriftart im WebControl ab

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForceValidation() {#getForceValidation--}
```
public boolean getForceValidation()
```


Ermittelt, ob die kundenseitige Validierung erzwungen wird.

**Remarks**

Wenn auf true gesetzt, werden Daten nicht an den Server gesendet, bis alle Eingabefelder gültig sind.

**Returns:**
boolean
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Ruft die Vordergrundfarbe im WebControl ab

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```


Ermittelt den Rahmenstil der Steuerung.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getGoonDefaultSaveOperation() {#getGoonDefaultSaveOperation--}
```
public boolean getGoonDefaultSaveOperation()
```


Ermittelt, ob GridWeb die Standard‑Speicheroperation ausführt, der Standardwert ist true.

**Returns:**
boolean
### getHeaderBarHeight() {#getHeaderBarHeight--}
```
public Unit getHeaderBarHeight()
```


Ermittelt die Höhe (System.Web.UI.WebControl.Unit) der oberen Kopfzeile der Steuerung.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeaderBarStyle() {#getHeaderBarStyle--}
```
public GridTableItemStyle getHeaderBarStyle()
```


Ermittelt den Stil der Kopfzeile.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```


Ermittelt den Stil der Kopfzeile der Steuerung.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarWidth() {#getHeaderBarWidth--}
```
public Unit getHeaderBarWidth()
```


Ermittelt die Breite (System.Web.UI.WebControl.Unit) der linken Kopfzeile der Steuerung.

**Example**

```
         		GridWeb1.setHeaderBarWidth(new Unit(32, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeaderBarHeight(new Unit(24, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Ermittelt die Höhe (System.Web.UI.WebControl.Unit) der Steuerung.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getIgnoreStyleWithNoData() {#getIgnoreStyleWithNoData--}
```
public boolean getIgnoreStyleWithNoData()
```


Ermittelt, ob GridWeb das Anzeigen von Zeilen oder Spalten, die keine Zellwerte enthalten, aber dennoch formatiert sind, ignoriert. Wenn auf true gesetzt, ist die Leistung besser. Der Standardwert ist false, was bedeutet, dass wir die letzte zusammenhängende Zeile/Spalte ohne Zellwerte, aber mit Formatierung, weiterhin anzeigen. Diese Option ist nur gültig, wenn EnableAsync false ist. Sie hat keine Wirkung, wenn EnableAsync true ist, was bedeutet, dass GridWeb alle Zeilen/Spalten mit Formatierung anzeigt.

**Returns:**
boolean
### getLoadOptions() {#getLoadOptions--}
```
public GridLoadOptions getLoadOptions()
```


Stellt die Ladeoptionen für GridWeb dar.

**Returns:**
[GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Ermittelt den maximalen Anzeigespaltenindex (nullbasiert) des Web‑Sheets. Die Steuerung verwendet den höheren Wert von MaxColumn und der maximalen Spalte der Sheet‑Daten.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Ermittelt den maximalen Anzeigereihenindex (nullbasiert) des Web‑Sheets. Die Steuerung verwendet den höheren Wert von MaxRow und der maximalen Zeile der Sheet‑Daten.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMessage() {#getMessage--}
```
public String getMessage()
```


Ermittelt die Meldung für das Raster.

**Returns:**
java.lang.String
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Ermittelt den minimalen Anzeigespaltenindex (nullbasiert) des Web‑Sheets. Die Steuerung verwendet den kleineren Wert von MinColumn und der minimalen Spalte der Sheet‑Daten.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


Ermittelt den minimalen Anzeigereihenindex (nullbasiert) des Web‑Sheets. Die Steuerung verwendet den kleineren Wert von MinRow und der minimalen Zeile der Sheet‑Daten.

**Example**

```
         		// Creates a 4x4 "display window".
         		GridWeb1.setMinRow(2);
         		GridWeb1.setMaxRow(5);
         		GridWeb1.setMinColumn(3);
         		GridWeb1.setMaxColumn(6);
```

**Returns:**
int
### getModifiedCells() {#getModifiedCells--}
```
public ArrayList getModifiedCells()
```


Ermittelt die Sammlung der vom Client modifizierten Zellen.

**Returns:**
java.util.ArrayList
### getNeedRenderGroupRows() {#getNeedRenderGroupRows--}
```
public boolean getNeedRenderGroupRows()
```


Ermittelt, ob Gruppenzeilen angezeigt werden.

**Returns:**
boolean
### getNoHScroll() {#getNoHScroll--}
```
public boolean getNoHScroll()
```


Ermittelt einen Wert, der angibt, ob die horizontale Bildlaufleiste ausgeblendet ist.

**Returns:**
boolean
### getNoScroll() {#getNoScroll--}
```
public boolean getNoScroll()
```


Ermittelt, ob die Bildlaufleiste angezeigt werden soll.

**Returns:**
boolean
### getNoVScroll() {#getNoVScroll--}
```
public boolean getNoVScroll()
```


Ermittelt einen Wert, der angibt, ob die vertikale Bildlaufleiste ausgeblendet ist.

**Returns:**
boolean
### getOnAjaxCallFinishedClientFunction() {#getOnAjaxCallFinishedClientFunction--}
```
public String getOnAjaxCallFinishedClientFunction()
```


Ermittelt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn ajaxcall abgeschlossen ist. Die Client‑Funktion sollte wie folgt deklariert werden:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnCellErrorClientFunction() {#getOnCellErrorClientFunction--}
```
public String getOnCellErrorClientFunction()
```


Ermittelt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn die Validierung einer Zelle fehlschlägt. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnCellSelectedAjaxCallBackClientFunction() {#getOnCellSelectedAjaxCallBackClientFunction--}
```
public String getOnCellSelectedAjaxCallBackClientFunction()
```


Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Zelle ausgewählt wird. Die Clientfunktion sollte wie folgt deklariert werden:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnCellSelectedClientFunction() {#getOnCellSelectedClientFunction--}
```
public String getOnCellSelectedClientFunction()
```


Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Zelle ausgewählt wird. Die Clientfunktion sollte wie folgt deklariert werden:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnCellUnselectedClientFunction() {#getOnCellUnselectedClientFunction--}
```
public String getOnCellUnselectedClientFunction()
```


Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Zelle deselektiert wird. Die Clientfunktion sollte wie folgt deklariert werden:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnCellUpdatedClientFunction() {#getOnCellUpdatedClientFunction--}
```
public String getOnCellUpdatedClientFunction()
```


Ermittelt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn der Wert einer Zelle aktualisiert wird. Die Clientfunktion sollte wie folgt deklariert werden:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnContextMenuShowClientFunction() {#getOnContextMenuShowClientFunction--}
```
public String getOnContextMenuShowClientFunction()
```


Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn das Kontextmenü angezeigt wird. Die Clientfunktion sollte wie folgt deklariert werden:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnDoubleClickCellClientFunction() {#getOnDoubleClickCellClientFunction--}
```
public String getOnDoubleClickCellClientFunction()
```


Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Zelle doppelt angeklickt wird. Die Clientfunktion sollte wie folgt deklariert werden:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnDoubleClickRowClientFunction() {#getOnDoubleClickRowClientFunction--}
```
public String getOnDoubleClickRowClientFunction()
```


Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Zeile doppelt angeklickt wird. Die Clientfunktion sollte wie folgt deklariert werden:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnGridInitClientFunction() {#getOnGridInitClientFunction--}
```
public String getOnGridInitClientFunction()
```


Ermittelt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn das Raster initialisiert wird. Die Clientfunktion sollte wie folgt deklariert werden:
function MyOnGridInit(grid)
\{
alert("The grid is initialized: " + grid.id);
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnPageChangeClientFunction() {#getOnPageChangeClientFunction--}
```
public String getOnPageChangeClientFunction()
```


Ermittelt die clientseitige Funktion, die nach einer Seitenindexänderung aufgerufen wird. Sie wirkt nur, wenn EnablePaging true ist. Die Clientfunktion sollte wie folgt deklariert werden:
function MyOnPageChange(index)
\{
console.log("current page is:"+index);
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnPageSubmitClientFunction() {#getOnPageSubmitClientFunction--}
```
public String getOnPageSubmitClientFunction()
```


Ermittelt die clientseitige Funktion, die aufgerufen wird, bevor die Seite clientseitig übermittelt wird.

**Returns:**
java.lang.String
### getOnShapeSelectedClientFunction() {#getOnShapeSelectedClientFunction--}
```
public String getOnShapeSelectedClientFunction()
```


Ermittelt die clientseitige Funktion, die aufgerufen wird, wenn eine Form ausgewählt wird. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnSubmitClientFunction() {#getOnSubmitClientFunction--}
```
public String getOnSubmitClientFunction()
```


Ermittelt die clientseitige Funktion, die aufgerufen wird, bevor das Steuerelement clientseitig übermittelt wird. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
Das arg ist das Übermittlungsargument und enthält den Befehl, der an den Server gesendet werden soll. Das cancelEdit ist ein boolescher Wert, der angibt, ob das Steuerelement die Benutzereingabe vor dem Senden verworfen hat. Das Steuerelement wird die Übermittlung fortsetzen, wenn die Funktion true zurückgibt.
Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Returns:**
java.lang.String
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Ermittelt, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist; der Standardwert ist false.

**Returns:**
boolean
### getPageSize() {#getPageSize--}
```
public int getPageSize()
```


Ermittelt die Seitengröße im Paging-Modus.

**Remarks**

Im Paging‑Modus zeigt das Steuerelement einmal PageSize Zeilen Daten an und stellt das Seitenwahl‑Steuerelement in der Registerkartenleiste dar.

**Returns:**
int
### getPictureCachePath() {#getPictureCachePath--}
```
public static String getPictureCachePath()
```


Ermittelt den Bildspeicherpfad für die Arbeitsmappe; alle Formen und Bilder werden in diesem Verzeichnis gespeichert. Der Standardpfad ist acwcache im Basisverzeichnis der aktuellen Anwendung. Benutzer müssen einen geplanten Dienst implementieren, um Dateien zu bereinigen, die die Sitzungszeit überschritten haben.

**Returns:**
java.lang.String
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Ermittelt den voreingestellten Stil.

Siehe [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Example**

```
         		GridWeb1.setPresetStyle(PresetStyle.TRADITIONAL_1);
```

**Returns:**
int
### getRefreshValidation() {#getRefreshValidation--}
```
public boolean getRefreshValidation()
```


Ermittelt, ob der Validierungswert nach einer Zellwertänderung aktualisiert werden soll.

**Returns:**
boolean
### getRenderHiddenRow() {#getRenderHiddenRow--}
```
public boolean getRenderHiddenRow()
```


Ermittelt, ob die versteckte Zeile in GridControl gerendert wird; der Standardwert ist false. Wenn Sie die versteckte Zeile später wieder einblenden müssen, sollten Sie sie auf true setzen.

**Returns:**
boolean
### getRowHeightForCSV() {#getRowHeightForCSV--}
```
public double getRowHeightForCSV()
```


Ermittelt den Zeilenhöhenwert in Punkt für CSV-Dateien; der Standardwert ist 14,5.

**Returns:**
double
### getScrollBarArrowColor() {#getScrollBarArrowColor--}
```
public Color getScrollBarArrowColor()
```


Gibt die Farbe der Pfeiltaste der Bildlaufleiste an.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getScrollBarBaseColor() {#getScrollBarBaseColor--}
```
public Color getScrollBarBaseColor()
```


Gibt die Farbe der Bildlaufleiste des Steuerelements an.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellBgColor() {#getSelectCellBgColor--}
```
public Color getSelectCellBgColor()
```


Gibt die Hintergrundfarbe der ausgewählten Zellen im Mehrfachauswahlbereich an.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellColor() {#getSelectCellColor--}
```
public Color getSelectCellColor()
```


Gibt die Farbe der ausgewählten Zellen im Mehrfachauswahlbereich an.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCells() {#getSelectCells--}
```
public ArrayList getSelectCells()
```


Ruft die Sammlung der ausgewählten Zellen ab.

**Returns:**
java.util.ArrayList
### getSessionStorePath() {#getSessionStorePath--}
```
public String getSessionStorePath()
```


Ruft den Pfad des Session-Cache-Speichers ab, wenn der Sitzungsmodus File oder ViewState usw. ist: gridweb.SessionStorePath="c:/mytempdir/session"; dann werden Sitzungsdaten in c:/mytempdir/session gespeichert.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Stellt die Arbeitsmappeneinstellungen dar.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings)
### getShowAddButton() {#getShowAddButton--}
```
public boolean getShowAddButton()
```


Ermittelt, ob die Schaltfläche zum Hinzufügen eines Arbeitsblatts angezeigt wird.

**Returns:**
boolean
### getShowBottomBar() {#getShowBottomBar--}
```
public boolean getShowBottomBar()
```


Gibt an, ob die Befehlsleiste (einschließlich Befehlsleiste und Registerkartenleiste) am unteren Rand des Steuerelements angezeigt wird.

**Returns:**
boolean
### getShowCellEditBox() {#getShowCellEditBox--}
```
public boolean getShowCellEditBox()
```


Gibt an, ob Gridweb die Symbolleiste für das Bearbeitungsfeld wie in MS‑EXCEL anzeigt. Wenn aktiviert, wird ein Bearbeitungsfeld für die aktuelle Zelle in Gridweb angezeigt. Wenn wir diese Funktion aktivieren, müssen Sie die jQuery‑JS‑Bibliothek in Ihre ASPX‑Dateien einbinden, um diese neue Funktion zu unterstützen. Jede aktuelle jQuery‑Version ist geeignet. usw.

**Returns:**
boolean
### getShowCommandBarAtTop() {#getShowCommandBarAtTop--}
```
public boolean getShowCommandBarAtTop()
```


Gibt an, ob die Befehlsleiste (einschließlich Befehlsleiste und Registerkartenleiste) am oberen Rand des Steuerelements angezeigt wird.

**Returns:**
boolean
### getShowContextMenu() {#getShowContextMenu--}
```
public boolean getShowContextMenu()
```


Ermittelt, ob das Kontextmenü angezeigt wird. Der Standardwert ist true.

**Returns:**
boolean
### getShowDefaultGridLine() {#getShowDefaultGridLine--}
```
public boolean getShowDefaultGridLine()
```


Ermittelt, ob die Standardgitternetzlinien der Zellen angezeigt werden.

**Returns:**
boolean
### getShowHeaderBar() {#getShowHeaderBar--}
```
public boolean getShowHeaderBar()
```


Ermittelt, ob die Kopfzeilenleiste angezeigt wird

**Returns:**
boolean
### getShowLoading() {#getShowLoading--}
```
public boolean getShowLoading()
```


Gibt an, ob während des Postbacks zum Server ein Lade-Dialogfeld angezeigt wird.

**Returns:**
boolean
### getShowLoadingPosition() {#getShowLoadingPosition--}
```
public String getShowLoadingPosition()
```


Gibt die linke, obere Position (in px) an, um das Lade-Dialogfeld während des Postbacks zum Server anzuzeigen usw. 100,200 bedeutet, dass die linke, obere Position des Lade-Dialogfelds bei 100px,200px liegt.

**Returns:**
java.lang.String
### getShowSaveButton() {#getShowSaveButton--}
```
public boolean getShowSaveButton()
```


Ermittelt, ob die Schaltfläche zum Speichern angezeigt wird.

**Returns:**
boolean
### getShowSubmitButton() {#getShowSubmitButton--}
```
public boolean getShowSubmitButton()
```


Ermittelt, ob die Schaltfläche zum Absenden angezeigt wird.

**Returns:**
boolean
### getShowTabBar() {#getShowTabBar--}
```
public boolean getShowTabBar()
```


Ermittelt, ob die Registerkartenleiste angezeigt wird.

**Returns:**
boolean
### getShowTabNavigation() {#getShowTabNavigation--}
```
public boolean getShowTabNavigation()
```


Ermittelt, ob die Registerkarten-Navigationsschaltfläche angezeigt wird, der Standardwert ist true.

**Returns:**
boolean
### getShowUndoButton() {#getShowUndoButton--}
```
public boolean getShowUndoButton()
```


Ermittelt, ob die Rückgängig-Schaltfläche angezeigt wird.

**Returns:**
boolean
### getSpanWrap() {#getSpanWrap--}
```
public boolean getSpanWrap()
```


Gibt an, ob der Inhalt im Zellenbereich umgebrochen wird. Der Standardwert ist true.

**Returns:**
boolean
### getTabIndex() {#getTabIndex--}
```
public short getTabIndex()
```


Ruft den TabIndex im WebControl ab

**Returns:**
short
### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```


Ermittelt den Stil der Registerkartenleiste.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Ruft den ToolTip im WebControl ab

**Returns:**
java.lang.String
### getUseClientPageHeight() {#getUseClientPageHeight--}
```
public boolean getUseClientPageHeight()
```


Ermittelt, ob Gridweb die Höhe der Client-Seite als Steuerelementhöhe verwendet, geeignet, wenn Height="100%" gesetzt ist, Standardwert ist false.

**Returns:**
boolean
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Ermittelt die Release‑Version.

**Returns:**
java.lang.String - Die Release-Version.
### getViewPanelScrollLeft() {#getViewPanelScrollLeft--}
```
public String getViewPanelScrollLeft()
```


Ermittelt die Position der Bildlaufleiste des Ansichtsbereichs des Rasters.

**Returns:**
java.lang.String
### getViewPanelScrollTop() {#getViewPanelScrollTop--}
```
public String getViewPanelScrollTop()
```


Ermittelt die Position der Bildlaufleiste des Ansichtsbereichs des Rasters.

**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```


Ermittelt den Stil des Datenansichtsbereichs.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Ermittelt die Breite (System.Web.UI.WebControl.Unit) des Steuerelements.

**Example**

```
         		GridWeb1.setWidth(new Unit(320, com.aspose.gridweb.UnitType.Point));
         		GridWeb1.setHeight(new Unit(240, com.aspose.gridweb.UnitType.Point));
```

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWorkSheets() {#getWorkSheets--}
```
public GridWorksheetCollection getWorkSheets()
```


Ermittelt die Sammlung der Arbeitsblätter.

**Returns:**
[GridWorksheetCollection](../../com.aspose.gridweb/gridworksheetcollection)
### getXhtmlMode() {#getXhtmlMode--}
```
public boolean getXhtmlMode()
```


Ermittelt, ob der XHTML-Stil verwendet wird, der Standardwert ist true.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importExcelFile(InputStream stream) {#importExcelFile-java.io.InputStream-}
```
public void importExcelFile(InputStream stream)
```


Importiert aus einem Excel-Datei-Stream, einschließlich Festplattendatei-Stream oder Speicher-Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der Stream der Excel‑Datei, einschließlich Dateistream von der Festplatte oder Memory‑Stream. |

### importExcelFile(InputStream stream, String passwordtoOpen) {#importExcelFile-java.io.InputStream-java.lang.String-}
```
public void importExcelFile(InputStream stream, String passwordtoOpen)
```


Importiert aus einem Excel-Datei-Stream, einschließlich Festplattendatei-Stream oder Speicher-Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der Stream der Excel‑Datei, einschließlich Dateistream von der Festplatte oder Memory‑Stream. |
| passwordtoOpen | java.lang.String | Das Öffnungspasswort für die verschlüsselte Datei. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Importiert aus einer Excel-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Name der Excel‑Datei. |

### importExcelFile(String fileName, String passwordtoOpen) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String fileName, String passwordtoOpen)
```


Importiert aus einer Excel-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Name der Excel‑Datei. |
| passwordtoOpen | java.lang.String | Das Öffnungspasswort für die verschlüsselte Datei. |

### isCalculateFormula() {#isCalculateFormula--}
```
public boolean isCalculateFormula()
```


Ermittelt, ob Formeln nach Änderungen des Zellenwerts oder nach dem Import einer Datei berechnet werden sollen. Der Standardwert ist true.

**Returns:**
boolean
### loadCSVFile(InputStream stream) {#loadCSVFile-java.io.InputStream-}
```
public void loadCSVFile(InputStream stream)
```


Lädt Daten aus einem CSV-Datei-Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der Dateistream. |

### loadCSVFile(String fileName) {#loadCSVFile-java.lang.String-}
```
public void loadCSVFile(String fileName)
```


Lädt Daten aus einer CSV-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Dateiname. |

### loadHTMLFile(InputStream stream) {#loadHTMLFile-java.io.InputStream-}
```
public void loadHTMLFile(InputStream stream)
```


Lädt Daten aus einem HTML-Datei-Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der Dateistream. |

### loadHTMLFile(String fileName) {#loadHTMLFile-java.lang.String-}
```
public void loadHTMLFile(String fileName)
```


Lädt Daten aus einer HTML-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Dateiname. |

### loadSpreadSheetMLFile(InputStream stream) {#loadSpreadSheetMLFile-java.io.InputStream-}
```
public void loadSpreadSheetMLFile(InputStream stream)
```


Lädt Daten aus einem SpreadSheetML-Datei-Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der Dateistream. |

### loadSpreadSheetMLFile(String fileName) {#loadSpreadSheetMLFile-java.lang.String-}
```
public void loadSpreadSheetMLFile(String fileName)
```


Lädt Daten aus einer SpreadSheetML-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Dateiname. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshChartShape() {#refreshChartShape--}
```
public void refreshChartShape()
```


Aktualisiert alle Diagrammbilder für das aktive Arbeitsblatt.

### saveCSVFile(OutputStream stream) {#saveCSVFile-java.io.OutputStream-}
```
public void saveCSVFile(OutputStream stream)
```


Speichert Daten in einen CSV-Datei-Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Dateistream. |

### saveCSVFile(String targetFile) {#saveCSVFile-java.lang.String-}
```
public void saveCSVFile(String targetFile)
```


Speichert Daten in einer CSV-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| targetFile | java.lang.String | Der Dateiname. |

### saveCustomStyleFile(String fileName) {#saveCustomStyleFile-java.lang.String-}
```
public void saveCustomStyleFile(String fileName)
```


Speichert die aktuellen Stildaten des Steuerelements in einer XML‑Datei. Kann verwendet werden, um Ihre benutzerdefinierte Stildatei zu erstellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Name der Stildatei. |

### saveHTMLFile(OutputStream stream) {#saveHTMLFile-java.io.OutputStream-}
```
public void saveHTMLFile(OutputStream stream)
```


Speichert Daten in einen HTML-Datei-Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Dateistream. |

### saveHTMLFile(String targetFile) {#saveHTMLFile-java.lang.String-}
```
public void saveHTMLFile(String targetFile)
```


Speichert Daten in einer HTML-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| targetFile | java.lang.String | Der Dateiname. |

### saveSpreadSheetMLFile(OutputStream stream) {#saveSpreadSheetMLFile-java.io.OutputStream-}
```
public void saveSpreadSheetMLFile(OutputStream stream)
```


Speichert Daten in einen SpreadSheetML-Datei-Stream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Dateistream. |

### saveSpreadSheetMLFile(String targetFile) {#saveSpreadSheetMLFile-java.lang.String-}
```
public void saveSpreadSheetMLFile(String targetFile)
```


Speichert Daten in einer SpreadSheetML-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| targetFile | java.lang.String | Der Dateiname. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Speichert die Arbeitsblätter in einer Excel-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Ziel‑Stream zum Schreiben. |

### saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions) {#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)
```


Speichert die Arbeitsblätter in einer Excel-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Ziel‑Stream zum Schreiben. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Die Speicheroptionen. |

### saveToExcelFile(OutputStream stream, int format) {#saveToExcelFile-java.io.OutputStream-int-}
```
public void saveToExcelFile(OutputStream stream, int format)
```


Speichert die Arbeitsblätter in einer Excel-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.OutputStream | Der Ziel‑Stream zum Schreiben. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Das Dateiformat (Excel2003, Excel2007, CSV, SpreadsheetML) |

### saveToExcelFile(String targetFile) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String targetFile)
```


Speichert die Arbeitsblätter in einer Excel-Datei im Excel‑2003‑Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| targetFile | java.lang.String | Der Name der Zieldatei, in die geschrieben werden soll. |

### saveToExcelFile(String targetFile, GridSaveOptions saveOptions) {#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(String targetFile, GridSaveOptions saveOptions)
```


Speichert die Arbeitsblätter in einer Excel-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| targetFile | java.lang.String | Der Name der Zieldatei, in die geschrieben werden soll. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Die Speicheroptionen. |

### saveToExcelFile(String targetFile, int format) {#saveToExcelFile-java.lang.String-int-}
```
public void saveToExcelFile(String targetFile, int format)
```


Speichert die Arbeitsblätter in einer Excel-Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| targetFile | java.lang.String | Der Name der Zieldatei, in die geschrieben werden soll. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Das Dateiformat (Excel2003, Excel2007, CSV, SpreadsheetML) |

### setACWClientPath(String value) {#setACWClientPath-java.lang.String-}
```
public void setACWClientPath(String value)
```


Legt den Webpfad der Skript-/Bilddateien des Steuerelements fest. Beispiel: "http://localhost/acw\_client". Sie können diesen Wert auch in der web.config-Datei festlegen. Fügen Sie diesen Abschnitt zum `<configuration>`-Abschnitt hinzu:
`<appSettings>`
`<add key=\"aspose.cells.gridweb.acw_client_path\" value=\"/acw_client/\" />`
`</appSettings>`


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setACWLanguageFileUrl(String value) {#setACWLanguageFileUrl-java.lang.String-}
```
public void setACWLanguageFileUrl(String value)
```


Legt die Web‑URL der Sprachdatei des Steuerelements fest. Beispiel: "/acw\_client/lang\_en.js".
Standardmäßig wird eine integrierte englische Datei verwendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setActiveCell(GridCell value) {#setActiveCell-com.aspose.gridweb.GridCell-}
```
public void setActiveCell(GridCell value)
```


Legt die aktive Zelle des aktuellen Arbeitsblatts fest. Seit Version 1.9.0.1 wurde sie schreibbar gemacht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```


Legt die Hintergrundfarbe der aktiven Zelle fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```


Legt die Farbe der aktiven Zelle fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```


Legt die Hintergrundfarbe der aktiven Zeilen-/Spaltenüberschrift fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```


Legt die Farbe der aktiven Zeilen-/Spaltenüberschrift fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Legt den Index des aktiven Arbeitsblatts fest. Entspricht WebWorksheets.ActiveSheetIndex.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```


Legt den Stil des aktiven Tabs fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoRefreshChart(boolean value) {#setAutoRefreshChart-boolean-}
```
public void setAutoRefreshChart(boolean value)
```


Legt fest, ob das Diagrammbild beim Aktualisieren des Zellenwerts aktualisiert wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


Legt die Hintergrundfarbe im WebControl fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Legt die Rahmenfarbe im WebControl fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Legt den Rahmenstil im WebControl fest

Siehe [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Legt die Rahmenbreite im WebControl fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```


Legt den Stil der unteren Leiste der Steuerung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Legt fest, ob Formeln nach Änderungen des Zellenwerts oder nach dem Import einer Datei berechnet werden sollen. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Setzt die CssClass im WebControl

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCurrentPageIndex(int value) {#setCurrentPageIndex-int-}
```
public void setCurrentPageIndex(int value)
```


Legt den aktuellen Seitenindex im Paging-Modus fest.

**Remarks**

Im Paging‑Modus zeigt das Steuerelement einmal PageSize Zeilen Daten an und stellt das Seitenwahl‑Steuerelement in der Registerkartenleiste dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCustomCalculationEngine(GridAbstractCalculationEngine value) {#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-}
```
public void setCustomCalculationEngine(GridAbstractCalculationEngine value)
```


Stellt die benutzerdefinierte Berechnungs‑Engine des Benutzers dar, um die Standard‑Berechnungs‑Engine von Aspose.Cells zu erweitern.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine) |  |

### setCustomStyle(InputStream stream) {#setCustomStyle-java.io.InputStream-}
```
public void setCustomStyle(InputStream stream)
```


Legt die benutzerdefinierte Stildatei aus einem Stream fest, einschließlich Dateistream von der Festplatte oder Speicherstream.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | java.io.InputStream | Der Stream der Datei, einschließlich Dateistream von der Festplatte oder Speicherstream. |

### setCustomStyleFileName(String value) {#setCustomStyleFileName-java.lang.String-}
```
public void setCustomStyleFileName(String value)
```


Legt den Namen der benutzerdefinierten Stildatei fest.

**Remarks**

Die benutzerdefinierte Stildatei ist eine XML-Datei. Wenn der Dateiname gesetzt wird, wird die Datei sofort geladen. Hier ist der Inhalt des "Standard-Voreinstellungsstils" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Ermittelt / legt die DPI des Geräts fest.

**Remarks**

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Legt den Standard‑Schriftartnamen des Steuerelements fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


Legt die Standard-Schriftgröße der Steuerung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```


Legt die Standardfarbe der Rasterlinien fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setDisplayCellTip(boolean value) {#setDisplayCellTip-boolean-}
```
public void setDisplayCellTip(boolean value)
```


Legt fest, ob Tipps angezeigt werden. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEditMode(boolean value) {#setEditMode-boolean-}
```
public void setEditMode(boolean value)
```


Legt den Bearbeitungsmodus der Steuerung fest.

**Remarks**

Wenn auf true gesetzt, sind die Zellen der Steuerung editierbar, und das "save"- und das "undo"-Symbol werden angezeigt. Wenn auf false gesetzt, sind die Zellen der Steuerung schreibgeschützt, und das "save"- und das "undo"-Symbol werden nicht angezeigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableAJAX(boolean value) {#setEnableAJAX-boolean-}
```
public void setEnableAJAX(boolean value)
```


Legt fest, ob ein AJAX-Aufruf verwendet wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableAsync(boolean value) {#setEnableAsync-boolean-}
```
public void setEnableAsync(boolean value)
```


Legt fest, ob Zellen-Daten asynchron geladen werden; empfohlen für ein Blatt mit mehr als 10.000 Zellen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableClientColumnOperations(boolean value) {#setEnableClientColumnOperations-boolean-}
```
public void setEnableClientColumnOperations(boolean value)
```


Legt fest, ob clientseitige Spaltenoperationen aktiviert werden.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer das Kontextmenü verwenden, um Spalten hinzuzufügen/zu entfernen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableClientFreeze(boolean value) {#setEnableClientFreeze-boolean-}
```
public void setEnableClientFreeze(boolean value)
```


Legt fest, ob clientseitige Freeze-Operationen aktiviert werden.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer das Kontextmenü verwenden, um Bereiche zu fixieren/zu lösen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableClientMergeOperations(boolean value) {#setEnableClientMergeOperations-boolean-}
```
public void setEnableClientMergeOperations(boolean value)
```


Legt fest, ob clientseitige Merge-Operationen aktiviert werden.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer das Kontextmenü verwenden, um Zellen zu verbinden/zu trennen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableClientResizeColumnRow(boolean value) {#setEnableClientResizeColumnRow-boolean-}
```
public void setEnableClientResizeColumnRow(boolean value)
```


Legt fest, ob das clientseitige Ändern der Größe von Spalten und Zeilen aktiviert wird.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer die Spalte und Zeile auf der Clientseite in der Größe anpassen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableClientRowOperations(boolean value) {#setEnableClientRowOperations-boolean-}
```
public void setEnableClientRowOperations(boolean value)
```


Legt fest, ob clientseitige Zeilenoperationen aktiviert werden.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer das Kontextmenü verwenden, um Zeilen hinzuzufügen/zu entfernen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableDoubleClickEvent(boolean value) {#setEnableDoubleClickEvent-boolean-}
```
public void setEnableDoubleClickEvent(boolean value)
```


Legt fest, ob das kundenseitige Doppelklick-Ereignis aktiviert wird.

**Remarks**

Wenn auf true gesetzt, empfängt die Steuerung clientseitige Doppelklick‑Ereignisse und Sie können diese Ereignisse auf der Serverseite verarbeiten. Andernfalls ignoriert die Steuerung alle Doppelklick‑Ereignisse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableMetalLightEffect(boolean value) {#setEnableMetalLightEffect-boolean-}
```
public void setEnableMetalLightEffect(boolean value)
```


Legt fest, ob der Metal-Light-Effekt angewendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnablePaging(boolean value) {#setEnablePaging-boolean-}
```
public void setEnablePaging(boolean value)
```


Legt fest, ob der Paging-Modus der Steuerung aktiviert wird.

**Remarks**

Wenn auf true gesetzt, zeigt die Steuerung einmal PageSize Zeilen Daten an und zeigt das Seiten‑Auswahl‑Steuerelement in der Tab‑Leiste an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnableStyleDialogbox(boolean value) {#setEnableStyleDialogbox-boolean-}
```
public void setEnableStyleDialogbox(boolean value)
```


Legt fest, ob das clientseitige Stil-Dialogfeld aktiviert wird.

**Remarks**

Wenn auf true gesetzt, kann der Benutzer das Stil‑Dialogfeld verwenden, um den Stil einer Zelle festzulegen, indem er im Kontextmenü "Format Cell..." auswählt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Setzt das Enabled im WebControl

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFilteredPaging(boolean value) {#setFilteredPaging-boolean-}
```
public void setFilteredPaging(boolean value)
```


Legt fest, ob das Paging nach Datenfilterung aktiviert wird; wirkt nur, wenn EnablePaging true ist.

**Remarks**

Wenn auf true gesetzt, paginiert die Steuerung basierend auf gefilterten Daten, der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Legt den Schriftarten-Ordner fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolder | java.lang.String | Der Ordner, der TrueType-Schriftarten enthält. |
| rekursiv | boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Setzt die Schriftordner

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Die Ordner, die TrueType-Schriften enthalten. |
| rekursiv | boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### setForceValidation(boolean value) {#setForceValidation-boolean-}
```
public void setForceValidation(boolean value)
```


Legt fest, ob die kundenseitige Validierung erzwungen wird.

**Remarks**

Wenn auf true gesetzt, werden Daten nicht an den Server gesendet, bis alle Eingabefelder gültig sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Setzt die ForeColor im WebControl

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```


Legt den Rahmenstil der Steuerung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setGoonDefaultSaveOperation(boolean value) {#setGoonDefaultSaveOperation-boolean-}
```
public void setGoonDefaultSaveOperation(boolean value)
```


Legt fest, ob GridWeb die Standard‑Speicheroperation ausführt, der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHeaderBarHeight(Unit value) {#setHeaderBarHeight-com.aspose.gridweb.Unit-}
```
public void setHeaderBarHeight(Unit value)
```


Legt die Höhe (System.Web.UI.WebControl.Unit) der oberen Kopfzeile der Steuerung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```


Legt den Stil der Kopfzeile fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```


Legt den Stil der Kopfzeilenleiste des Steuerelements fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setHeaderBarWidth(Unit value) {#setHeaderBarWidth-com.aspose.gridweb.Unit-}
```
public void setHeaderBarWidth(Unit value)
```


Legt die Breite ( System.Web.UI.WebControl.Unit ) oder die linke Kopfzeilenleiste des Steuerelements fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Legt die Höhe ( System.Web.UI.WebControl.Unit ) des Steuerelements fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setIgnoreStyleWithNoData(boolean value) {#setIgnoreStyleWithNoData-boolean-}
```
public void setIgnoreStyleWithNoData(boolean value)
```


Legt fest, ob GridWeb das Anzeigen von Zeilen oder Spalten, die keine Zellenwerte enthalten, aber dennoch formatiert sind, ignoriert. Wenn auf true gesetzt, ist die Leistung besser. Der Standardwert ist false, was bedeutet, dass wir letzte zusammenhängende Zeilen/Spalten ohne Zellenwerte, aber mit Formatierung, weiterhin anzeigen. Diese Option ist nur gültig, wenn EnableAsync false ist. Sie hat keine Wirkung, wenn EnableAsync true ist, was bedeutet, dass GridWeb alle Zeilen/Spalten mit Formatierung anzeigt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLoadOptions(GridLoadOptions value) {#setLoadOptions-com.aspose.gridweb.GridLoadOptions-}
```
public void setLoadOptions(GridLoadOptions value)
```


Stellt die Ladeoptionen für GridWeb dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridLoadOptions](../../com.aspose.gridweb/gridloadoptions) |  |

### setMaxColumn(int value) {#setMaxColumn-int-}
```
public void setMaxColumn(int value)
```


Legt den maximalen Anzeigespaltenindex (nullbasiert) des Webblatts fest. Das Steuerelement verwendet den größeren Wert von MaxColumn und dem maximalen Spaltenwert der Blattdaten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMaxRow(int value) {#setMaxRow-int-}
```
public void setMaxRow(int value)
```


Legt den maximalen Anzeigereihenindex (nullbasiert) des Webblatts fest. Das Steuerelement verwendet den größeren Wert von MaxRow und dem maximalen Reihenwert der Blattdaten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMessage(String value) {#setMessage-java.lang.String-}
```
public void setMessage(String value)
```


Legt die Meldung für das Raster fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setMinColumn(int value) {#setMinColumn-int-}
```
public void setMinColumn(int value)
```


Legt den minimalen Anzeigespaltenindex (nullbasiert) des Webblatts fest. Das Steuerelement verwendet den kleineren Wert von MinColumn und dem minimalen Spaltenwert der Blattdaten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setMinRow(int value) {#setMinRow-int-}
```
public void setMinRow(int value)
```


Legt den minimalen Anzeigereihenindex (nullbasiert) des Webblatts fest. Das Steuerelement verwendet den kleineren Wert von MinRow und dem minimalen Reihenwert der Blattdaten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setNeedRenderGroupRows(boolean value) {#setNeedRenderGroupRows-boolean-}
```
public void setNeedRenderGroupRows(boolean value)
```


Legt fest, ob Gruppenzeilen angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setNoHScroll(boolean value) {#setNoHScroll-boolean-}
```
public void setNoHScroll(boolean value)
```


Legt einen Wert fest, der angibt, ob die horizontale Bildlaufleiste ausgeblendet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setNoScroll(boolean value) {#setNoScroll-boolean-}
```
public void setNoScroll(boolean value)
```


Legt fest, ob die Bildlaufleiste angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setNoVScroll(boolean value) {#setNoVScroll-boolean-}
```
public void setNoVScroll(boolean value)
```


Legt einen Wert fest, der angibt, ob die vertikale Bildlaufleiste ausgeblendet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOnAjaxCallFinishedClientFunction(String value) {#setOnAjaxCallFinishedClientFunction-java.lang.String-}
```
public void setOnAjaxCallFinishedClientFunction(String value)
```


Legt den Namen der clientseitigen Funktion fest, die aufgerufen wird, wenn der Ajax‑Aufruf abgeschlossen ist. Die Client‑Funktion sollte wie folgt deklariert werden:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnCellErrorClientFunction(String value) {#setOnCellErrorClientFunction-java.lang.String-}
```
public void setOnCellErrorClientFunction(String value)
```


Legt den Namen der clientseitigen Funktion fest, die aufgerufen wird, wenn die Validierung einer Zelle fehlschlägt. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnCellSelectedAjaxCallBackClientFunction(String value) {#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-}
```
public void setOnCellSelectedAjaxCallBackClientFunction(String value)
```


Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zelle ausgewählt wird. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnCellSelectedClientFunction(String value) {#setOnCellSelectedClientFunction-java.lang.String-}
```
public void setOnCellSelectedClientFunction(String value)
```


Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zelle ausgewählt wird. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnCellUnselectedClientFunction(String value) {#setOnCellUnselectedClientFunction-java.lang.String-}
```
public void setOnCellUnselectedClientFunction(String value)
```


Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zelle deselektiert wird. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnCellUpdatedClientFunction(String value) {#setOnCellUpdatedClientFunction-java.lang.String-}
```
public void setOnCellUpdatedClientFunction(String value)
```


Legt den Namen der clientseitigen Funktion fest, die aufgerufen wird, wenn der Wert einer Zelle aktualisiert wird. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnContextMenuShowClientFunction(String value) {#setOnContextMenuShowClientFunction-java.lang.String-}
```
public void setOnContextMenuShowClientFunction(String value)
```


Legt die clientseitige Funktion fest, die aufgerufen wird, wenn das Kontextmenü angezeigt wird. Die Client‑Funktion sollte wie folgt deklariert werden:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnDoubleClickCellClientFunction(String value) {#setOnDoubleClickCellClientFunction-java.lang.String-}
```
public void setOnDoubleClickCellClientFunction(String value)
```


Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zelle doppelt angeklickt wird. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnDoubleClickRowClientFunction(String value) {#setOnDoubleClickRowClientFunction-java.lang.String-}
```
public void setOnDoubleClickRowClientFunction(String value)
```


Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Zeile doppelt angeklickt wird. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnGridInitClientFunction(String value) {#setOnGridInitClientFunction-java.lang.String-}
```
public void setOnGridInitClientFunction(String value)
```


Legt den Namen der clientseitigen Funktion fest, die aufgerufen wird, wenn das Raster initialisiert wird. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnGridInit(grid)
\{
alert("The grid is initialized: " + grid.id);
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnPageChangeClientFunction(String value) {#setOnPageChangeClientFunction-java.lang.String-}
```
public void setOnPageChangeClientFunction(String value)
```


Legt die clientseitige Funktion fest, die nach einer Seitenindexänderung aufgerufen wird. Wirkt nur, wenn EnablePaging true ist. Die Client‑Funktion sollte wie folgt deklariert werden:
function MyOnPageChange(index)
\{
console.log("current page is:"+index);
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnPageSubmitClientFunction(String value) {#setOnPageSubmitClientFunction-java.lang.String-}
```
public void setOnPageSubmitClientFunction(String value)
```


Legt die clientseitige Funktion fest, die aufgerufen wird, bevor die Seite clientseitig übermittelt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnShapeSelectedClientFunction(String value) {#setOnShapeSelectedClientFunction-java.lang.String-}
```
public void setOnShapeSelectedClientFunction(String value)
```


Legt die clientseitige Funktion fest, die aufgerufen wird, wenn eine Form ausgewählt wird. Die Clientfunktion sollte wie folgt deklariert werden:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnSubmitClientFunction(String value) {#setOnSubmitClientFunction-java.lang.String-}
```
public void setOnSubmitClientFunction(String value)
```


Legt die clientseitige Funktion fest, die aufgerufen wird, bevor das Steuerelement clientseitig übermittelt wird. Die Clientfunktion sollte wie folgt deklariert werden:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
Das arg ist das Übermittlungsargument und enthält den Befehl, der an den Server gesendet werden soll. Das cancelEdit ist ein boolescher Wert, der angibt, ob das Steuerelement die Benutzereingabe vor dem Senden verworfen hat. Das Steuerelement wird die Übermittlung fortsetzen, wenn die Funktion true zurückgibt.
Hinweis: Sie können den "this"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Legt fest, ob nur die Zeilen angepasst werden, deren Höhe nicht benutzerdefiniert ist; der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setPageSize(int value) {#setPageSize-int-}
```
public void setPageSize(int value)
```


Legt die Seitengröße im Paging-Modus fest.

**Remarks**

Im Paging‑Modus zeigt das Steuerelement einmal PageSize Zeilen Daten an und stellt das Seitenwahl‑Steuerelement in der Registerkartenleiste dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPictureCachePath(String value) {#setPictureCachePath-java.lang.String-}
```
public static void setPictureCachePath(String value)
```


Legt den Bildspeicherpfad für die Arbeitsmappe fest, alle Formen und Bilder werden in diesem Verzeichnis gespeichert; der Standardpfad ist acwcache im Basisverzeichnis der aktuellen Anwendung. Benutzer müssen einen geplanten Dienst implementieren, um Dateien zu bereinigen, die die Sitzungszeit überschritten haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Legt den voreingestellten Stil fest.

Siehe [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setRefreshValidation(boolean value) {#setRefreshValidation-boolean-}
```
public void setRefreshValidation(boolean value)
```


Legt fest, ob der Validierungswert nach Änderungen des Zellenwerts aktualisiert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRenderHiddenRow(boolean value) {#setRenderHiddenRow-boolean-}
```
public void setRenderHiddenRow(boolean value)
```


Legt fest, ob die versteckte Zeile im GridControl gerendert wird, der Standardwert ist false. Wenn Sie die versteckte Zeile später wieder einblenden müssen, sollten Sie sie auf true setzen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRowHeightForCSV(double value) {#setRowHeightForCSV-double-}
```
public void setRowHeightForCSV(double value)
```


Legt den Zeilenhöhenwert in Punkt für CSV-Dateien fest, Standardwert ist 14,5.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```


Gibt die Farbe der Pfeiltaste der Bildlaufleiste an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```


Gibt die Farbe der Bildlaufleiste des Steuerelements an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```


Gibt die Hintergrundfarbe der ausgewählten Zellen im Mehrfachauswahlbereich an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```


Gibt die Farbe der ausgewählten Zellen im Mehrfachauswahlbereich an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSessionStorePath(String value) {#setSessionStorePath-java.lang.String-}
```
public void setSessionStorePath(String value)
```


Legt den Pfad für den Sitzungs-Cache fest, wenn der Sitzungsmodus File oder ViewState ist usw.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; anschließend werden Sitzungsdaten in c:/mytempdir/session gespeichert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridweb.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Stellt die Arbeitsmappeneinstellungen dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings) |  |

### setShowAddButton(boolean value) {#setShowAddButton-boolean-}
```
public void setShowAddButton(boolean value)
```


Legt fest, ob die Schaltfläche zum Hinzufügen eines Arbeitsblatts angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowBottomBar(boolean value) {#setShowBottomBar-boolean-}
```
public void setShowBottomBar(boolean value)
```


Gibt an, ob die Befehlsleiste (einschließlich Befehlsleiste und Registerkartenleiste) am unteren Rand des Steuerelements angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowCellEditBox(boolean value) {#setShowCellEditBox-boolean-}
```
public void setShowCellEditBox(boolean value)
```


Gibt an, ob Gridweb die Symbolleiste für das Bearbeitungsfeld wie in MS‑EXCEL anzeigt. Wenn aktiviert, wird ein Bearbeitungsfeld für die aktuelle Zelle in Gridweb angezeigt. Wenn wir diese Funktion aktivieren, müssen Sie die jQuery‑JS‑Bibliothek in Ihre ASPX‑Dateien einbinden, um diese neue Funktion zu unterstützen. Jede aktuelle jQuery‑Version ist geeignet. usw.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowCommandBarAtTop(boolean value) {#setShowCommandBarAtTop-boolean-}
```
public void setShowCommandBarAtTop(boolean value)
```


Gibt an, ob die Befehlsleiste (einschließlich Befehlsleiste und Registerkartenleiste) am oberen Rand des Steuerelements angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowContextMenu(boolean value) {#setShowContextMenu-boolean-}
```
public void setShowContextMenu(boolean value)
```


Legt fest, ob das Kontextmenü angezeigt wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowDefaultGridLine(boolean value) {#setShowDefaultGridLine-boolean-}
```
public void setShowDefaultGridLine(boolean value)
```


Legt fest, ob die Standardgitterlinien der Zellen angezeigt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowHeaderBar(boolean value) {#setShowHeaderBar-boolean-}
```
public void setShowHeaderBar(boolean value)
```


Legt fest, ob die Header-Leiste angezeigt wird

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowLoading(boolean value) {#setShowLoading-boolean-}
```
public void setShowLoading(boolean value)
```


Gibt an, ob während des Postbacks zum Server ein Lade-Dialogfeld angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowLoadingPosition(String value) {#setShowLoadingPosition-java.lang.String-}
```
public void setShowLoadingPosition(String value)
```


Gibt die linke, obere Position (in px) an, um das Lade-Dialogfeld während des Postbacks zum Server anzuzeigen usw. 100,200 bedeutet, dass die linke, obere Position des Lade-Dialogfelds bei 100px,200px liegt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setShowSaveButton(boolean value) {#setShowSaveButton-boolean-}
```
public void setShowSaveButton(boolean value)
```


Legt fest, ob die Schaltfläche zum Speichern angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowSubmitButton(boolean value) {#setShowSubmitButton-boolean-}
```
public void setShowSubmitButton(boolean value)
```


Legt fest, ob die Schaltfläche zum Absenden angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowTabBar(boolean value) {#setShowTabBar-boolean-}
```
public void setShowTabBar(boolean value)
```


Legt fest, ob die Registerkartenleiste angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowTabNavigation(boolean value) {#setShowTabNavigation-boolean-}
```
public void setShowTabNavigation(boolean value)
```


Legt fest, ob die Registerkarten-Navigationsschaltfläche angezeigt wird; der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setShowUndoButton(boolean value) {#setShowUndoButton-boolean-}
```
public void setShowUndoButton(boolean value)
```


Legt fest, ob die Rückgängig-Schaltfläche angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSpanWrap(boolean value) {#setSpanWrap-boolean-}
```
public void setSpanWrap(boolean value)
```


Gibt an, ob der Inhalt im Zellenbereich umgebrochen wird. Der Standardwert ist true.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTabIndex(short value) {#setTabIndex-short-}
```
public void setTabIndex(short value)
```


Setzt den TabIndex im WebControl

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | short |  |

### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```


Legt den Stil der Registerkartenleiste fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Setzt den ToolTip im WebControl

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setUseClientPageHeight(boolean value) {#setUseClientPageHeight-boolean-}
```
public void setUseClientPageHeight(boolean value)
```


Legt fest, ob GridWeb die Höhe der Clientseite als Steuerungshöhe verwendet, geeignet für die Einstellung Height=\"100%\"; der Standardwert ist false.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setViewPanelScrollLeft(String value) {#setViewPanelScrollLeft-java.lang.String-}
```
public void setViewPanelScrollLeft(String value)
```


Legt die Position der Bildlaufleiste des Ansichtsbereichs des Rasters fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setViewPanelScrollTop(String value) {#setViewPanelScrollTop-java.lang.String-}
```
public void setViewPanelScrollTop(String value)
```


Legt die Position der Bildlaufleiste des Ansichtsbereichs des Rasters fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```


Legt den Stil des Datenansichtsbereichs fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Legt die Breite (System.Web.UI.WebControl.Unit) der Steuerung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setXhtmlMode(boolean value) {#setXhtmlMode-boolean-}
```
public void setXhtmlMode(boolean value)
```


Legt fest, ob der XHTML-Stil verwendet wird; der Standardwert ist true.

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

