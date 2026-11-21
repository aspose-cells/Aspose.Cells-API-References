---
title: "GridWeb"
second_title: "Aspose.Cells för Java API-referens"
description: "Den grundläggande klassen för GridWeb-kontrollen."
type: docs
url: /sv/java/com.aspose.gridweb/gridweb/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebControl](../../com.aspose.gridweb/webcontrol), [com.aspose.gridweb.ExtWebControl](../../com.aspose.gridweb/extwebcontrol), [com.aspose.gridweb.MainWeb](../../com.aspose.gridweb/mainweb)
```
public class GridWeb extends MainWeb
```

Den grundläggande klassen för GridWeb-kontrollen.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [GridWeb()](#GridWeb--) |  |
## Fält

| Fält | Beskrivning |
| --- | --- |
| [AfterColumnFilter](#AfterColumnFilter) | Uppstår efter att kolumnen filtrerats. |
| [AjaxCallFinished](#AjaxCallFinished) | Utlöses när ajax‑uppdateringen av kontrollen är klar. |
| [BeforeColumnFilter](#BeforeColumnFilter) | Uppstår innan kolumnen ska filtreras. |
| [CellClickOnAjax](#CellClickOnAjax) | Uppstår när cellen klickas, och ett ajaxcallback behövs för denna händelse. |
| [CellClientUpdate](#CellClientUpdate) | Uppstår när en klientcellsuppdatering sker. |
| [CellCommand](#CellCommand) | Uppstår när en cells kommando‑hyperlänk klickas. |
| [CellDoubleClick](#CellDoubleClick) | Uppstår när cellen dubbelklickas. |
| [CellModifiedOnAjax](#CellModifiedOnAjax) | Uppstår när cellen ändras i ajaxcall. |
| [ColumnDeleted](#ColumnDeleted) | Uppstår när användaren tar bort en kolumn från den klient‑baserade menyn. |
| [ColumnDeleting](#ColumnDeleting) | Uppstår när användaren försöker ta bort en kolumn från den klientbaserade menyn. |
| [ColumnDoubleClick](#ColumnDoubleClick) | Uppstår när kolumnrubriken dubbelklickas. |
| [ColumnInserted](#ColumnInserted) | Uppstår när användaren infogar en kolumn från den klientbaserade menyn. |
| [CustomCommand](#CustomCommand) | Uppstår när användaren klickar på en anpassad kommandoknapp. |
| [LoadCustomData](#LoadCustomData) | Utlöses när kontrollens SessionMode är inställd på Custom och behöver ladda bladdata. |
| [PageIndexChanged](#PageIndexChanged) | Uppstår när kontrollens bladsidindex har ändrats. |
| [RowDeleted](#RowDeleted) | Uppstår när användaren har tagit bort en rad från den klientbaserade menyn. |
| [RowDeleting](#RowDeleting) | Uppstår när användaren försöker ta bort en rad från den klientbaserade menyn. |
| [RowDoubleClick](#RowDoubleClick) | Uppstår när radrubriken dubbelklickas. |
| [RowInserted](#RowInserted) | Uppstår när användaren infogar en rad från den klientbaserade menyn. |
| [SaveCommand](#SaveCommand) | Uppstår när "spara"-knappen klickas. |
| [SheetAdded](#SheetAdded) | Uppstår när användaren lägger till ett arbetsblad från verktygsfältets meny. |
| [SheetTabClick](#SheetTabClick) | Uppstår när bladfliken klickas. |
| [SubmitCommand](#SubmitCommand) | Uppstår när "skicka"-knappen klickas. |
| [UndoCommand](#UndoCommand) | Uppstår när "ångra"-knappen klickas. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [calculateFormula()](#calculateFormula--) | Beräknar resultatet av formler. |
| [createChildControls()](#createChildControls--) | implementera CreateChildControls från WebControl, endast för internt bruk. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getACWClientPath()](#getACWClientPath--) | Hämtar webbvägen för skript-/bildfilerna för kontrollen. |
| [getACWLanguageFileUrl()](#getACWLanguageFileUrl--) | Hämtar webb‑URL för språkfilen för kontrollen. |
| [getActiveCell()](#getActiveCell--) | Hämtar den aktiva cellen i det aktuella bladet. |
| [getActiveCellBgColor()](#getActiveCellBgColor--) | Anger bakgrundsfärgen för den aktiva cellen. |
| [getActiveCellColor()](#getActiveCellColor--) | Anger färgen för den aktiva cellen. |
| [getActiveHeaderBgColor()](#getActiveHeaderBgColor--) | Anger bakgrundsfärgen för den aktiva rad‑/kolumnrubriken. |
| [getActiveHeaderColor()](#getActiveHeaderColor--) | Anger färgen för den aktiva rad‑/kolumnrubriken. |
| [getActiveSheet()](#getActiveSheet--) | Hämtar det aktiva bladet |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Hämtar indexet för det aktiva bladet. |
| [getActiveTabStyle()](#getActiveTabStyle--) | Anger stilen för den aktiva fliken. |
| [getAutoRefreshChart()](#getAutoRefreshChart--) | Hämtar om diagrambilden uppdateras medan cellvärdet uppdateras. standardvärdet är true |
| [getBackColor()](#getBackColor--) | Hämtar BackColor i WebControl |
| [getBorderColor()](#getBorderColor--) | Hämtar BorderColor i WebControl |
| [getBorderStyle()](#getBorderStyle--) | Hämtar BorderStyle i WebControl |
| [getBorderWidth()](#getBorderWidth--) | Hämtar BorderWidth i WebControl |
| [getBottomTableStyle()](#getBottomTableStyle--) | Hämtar stilen för kontrollens nedre stapel. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Hämtar CssClass i WebControl |
| [getCurrentPageIndex()](#getCurrentPageIndex--) | Hämtar det aktuella sidindexet i pagineringsläge. |
| [getCustomCalculationEngine()](#getCustomCalculationEngine--) | Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells. |
| [getCustomCommandButtons()](#getCustomCommandButtons--) | Hämtar den anpassade samlingen av kommandoknappar |
| [getCustomStyleFileName()](#getCustomStyleFileName--) | Hämtar det anpassade stilfilnamnet. |
| [getDPI()](#getDPI--) | Hämtar /Ställer in DPI för maskinen. |
| [getDefaultFontName()](#getDefaultFontName--) | Hämtar kontrollens standardteckensnittsnamn. |
| [getDefaultFontSize()](#getDefaultFontSize--) | Hämtar kontrollens standardteckenstorlek. |
| [getDefaultGridLineColor()](#getDefaultGridLineColor--) | Hämtar standardrutnätslinjens färg. |
| [getDisplayCellTip()](#getDisplayCellTip--) | Hämtar om tips ska visas. standardvärdet är true. |
| [getEditMode()](#getEditMode--) | Hämtar kontrollens redigeringsläge. |
| [getEnableAJAX()](#getEnableAJAX--) | Hämtar om AJAX-anrop ska användas. standardvärdet är true. |
| [getEnableAsync()](#getEnableAsync--) | Hämtar om celldata laddas asynkront, föreslås för ett blad med mer än 10000 celler. |
| [getEnableClientColumnOperations()](#getEnableClientColumnOperations--) | Hämtar om kolumnoperationer på klientsidan ska aktiveras. |
| [getEnableClientFreeze()](#getEnableClientFreeze--) | Hämtar om frysningsoperationer på klientsidan ska aktiveras. |
| [getEnableClientMergeOperations()](#getEnableClientMergeOperations--) | Hämtar om sammanslagningsoperationer på klientsidan ska aktiveras. |
| [getEnableClientResizeColumnRow()](#getEnableClientResizeColumnRow--) | Hämtar om ändring av kolumn- och radstorlek på klientsidan ska aktiveras. |
| [getEnableClientRowOperations()](#getEnableClientRowOperations--) | Hämtar om radoperationer på klientsidan ska aktiveras. |
| [getEnableDoubleClickEvent()](#getEnableDoubleClickEvent--) | Hämtar om kundsidans dubbelklickshändelse ska aktiveras. |
| [getEnableMetalLightEffect()](#getEnableMetalLightEffect--) | Hämtar om metallljuseffekt ska tillämpas. |
| [getEnablePaging()](#getEnablePaging--) | Hämtar om kontrollens pagineringsläge ska aktiveras. |
| [getEnableStyleDialogbox()](#getEnableStyleDialogbox--) | Hämtar om stil‑dialogrutan på klientsidan ska aktiveras. |
| [getEnabled()](#getEnabled--) | Hämtar Enabled i WebControl |
| [getFilteredPaging()](#getFilteredPaging--) | Hämtar om paginering ska aktiveras efter att data filtrerats, träder i kraft när EnablePaging är true. |
| [getFont()](#getFont--) | Hämtar Font i WebControl |
| [getForceValidation()](#getForceValidation--) | Hämtar om kundsidans validering ska tvingas. |
| [getForeColor()](#getForeColor--) | Hämtar ForeColor i WebControl |
| [getFrameTableStyle()](#getFrameTableStyle--) | Hämtar ramstilen för kontrollen. |
| [getGoonDefaultSaveOperation()](#getGoonDefaultSaveOperation--) | Hämtar om GridWeb kommer att utföra standard‑sparåtgärden, standardvärdet är true. |
| [getHeaderBarHeight()](#getHeaderBarHeight--) | Hämtar höjden( System.Web.UI.WebControl.Unit ) för kontrollens översta rubrikfält. |
| [getHeaderBarStyle()](#getHeaderBarStyle--) | Hämtar rubrikfältets stil. |
| [getHeaderBarTableStyle()](#getHeaderBarTableStyle--) | Hämtar rubrikfältets stil för kontrollen. |
| [getHeaderBarWidth()](#getHeaderBarWidth--) | Hämtar bredden( System.Web.UI.WebControl.Unit ) för kontrollens vänstra rubrikfält. |
| [getHeight()](#getHeight--) | Hämtar höjden( System.Web.UI.WebControl.Unit ) för kontrollen. |
| [getIgnoreStyleWithNoData()](#getIgnoreStyleWithNoData--) | Hämtar om GridWeb ignorerar att visa rader eller kolumner som inte innehåller cellvärden men ändå är formaterade. |
| [getLoadOptions()](#getLoadOptions--) | Representerar laddningsalternativen för GridWeb. |
| [getMaxColumn()](#getMaxColumn--) | Hämtar det maximala visningskolumnindexet (nollbaserat) för webbläsarket. |
| [getMaxRow()](#getMaxRow--) | Hämtar det maximala visningsradindexet (nollbaserat) för webbläsarket. |
| [getMessage()](#getMessage--) | Hämtar meddelandet för rutnätet. |
| [getMinColumn()](#getMinColumn--) | Hämtar det minsta visningskolumnindexet (nollbaserat) för webbläsarket. |
| [getMinRow()](#getMinRow--) | Hämtar det minsta visningsradindexet (nollbaserat) för webbläsarket. |
| [getModifiedCells()](#getModifiedCells--) | Hämtar samlingen av celler som har modifierats av klienten. |
| [getNeedRenderGroupRows()](#getNeedRenderGroupRows--) | Hämtar om grouprows ska visas. |
| [getNoHScroll()](#getNoHScroll--) | Hämtar ett värde som indikerar om den horisontella rullningslisten är dold. |
| [getNoScroll()](#getNoScroll--) | Hämtar om rullningslisten ska visas. |
| [getNoVScroll()](#getNoVScroll--) | Hämtar ett värde som indikerar om den vertikala rullningslisten är dold. |
| [getOnAjaxCallFinishedClientFunction()](#getOnAjaxCallFinishedClientFunction--) | Hämtar klient‑sidans funktionsnamn som ska anropas när ajax‑anropet är slutfört. |
| [getOnCellErrorClientFunction()](#getOnCellErrorClientFunction--) | Hämtar klient‑sidans funktionsnamn som ska anropas när en cells validering misslyckas. |
| [getOnCellSelectedAjaxCallBackClientFunction()](#getOnCellSelectedAjaxCallBackClientFunction--) | Hämtar klient‑sidans funktion som ska anropas när en cell har markerats. |
| [getOnCellSelectedClientFunction()](#getOnCellSelectedClientFunction--) | Hämtar klient‑sidans funktion som ska anropas när en cell har markerats. |
| [getOnCellUnselectedClientFunction()](#getOnCellUnselectedClientFunction--) | Hämtar klient‑sidans funktion som ska anropas när en cell har avmarkerats. |
| [getOnCellUpdatedClientFunction()](#getOnCellUpdatedClientFunction--) | Hämtar klient‑sidans funktionsnamn som ska anropas när en cells värde har uppdaterats. |
| [getOnContextMenuShowClientFunction()](#getOnContextMenuShowClientFunction--) | Hämtar klient‑sidans funktion som ska anropas när snabbmenyn ska visas. |
| [getOnDoubleClickCellClientFunction()](#getOnDoubleClickCellClientFunction--) | Hämtar klient‑sidans funktion som ska anropas när en cell dubbelklickas. |
| [getOnDoubleClickRowClientFunction()](#getOnDoubleClickRowClientFunction--) | Hämtar klient‑sidans funktion som ska anropas när en rad dubbelklickas. |
| [getOnGridInitClientFunction()](#getOnGridInitClientFunction--) | Hämtar namnet på klient‑sidans funktion som ska anropas när rutnätet initieras. |
| [getOnPageChangeClientFunction()](#getOnPageChangeClientFunction--) | Hämtar klient‑sidans funktion som ska anropas efter att sidindex har ändrats. Gäller endast när EnablePaging är true. |
| [getOnPageSubmitClientFunction()](#getOnPageSubmitClientFunction--) | Hämtar klientfunktionen som ska anropas innan sidan skickas in på klientsidan. |
| [getOnShapeSelectedClientFunction()](#getOnShapeSelectedClientFunction--) | Hämtar klient‑sidans funktion som ska anropas när en form väljs. |
| [getOnSubmitClientFunction()](#getOnSubmitClientFunction--) | Hämtar klientfunktionen som ska anropas innan kontrollen skickas in på klientsidan. |
| [getOnlyAuto()](#getOnlyAuto--) | Hämtar om endast rader vars höjd inte är anpassad ska passa, standardvärdet är false. |
| [getPageSize()](#getPageSize--) | Hämtar sidstorleken i pagineringsläge. |
| [getPictureCachePath()](#getPictureCachePath--) | Hämtar bildlagringssökvägen för arbetsboken, alla former och bilder lagras i denna katalog, standardsökvägen är acwcache under den aktuella applikationens baskatalog. Användare måste implementera en schemalagd tjänst för att rensa filer som har gått utanför sessionstiden. |
| [getPresetStyle()](#getPresetStyle--) | Hämtar den förinställda stilen. |
| [getRefreshValidation()](#getRefreshValidation--) | Hämtar om valideringsvärdet ska uppdateras efter att cellvärdet ändras. |
| [getRenderHiddenRow()](#getRenderHiddenRow--) | Hämtar om den dolda raden renderas i GridControl, standardvärdet är false. |
| [getRowHeightForCSV()](#getRowHeightForCSV--) | Hämtar radens höjdvärde i punkter för csv‑fil, standardvärdet är 14,5. |
| [getScrollBarArrowColor()](#getScrollBarArrowColor--) | Anger färgen på rullningslistens pilknapp. |
| [getScrollBarBaseColor()](#getScrollBarBaseColor--) | Anger färgen på kontrollens rullningslist. |
| [getSelectCellBgColor()](#getSelectCellBgColor--) | Anger bakgrundsfärgen för de markerade cellerna i ett flervalsområde. |
| [getSelectCellColor()](#getSelectCellColor--) | Anger färgen på de markerade cellerna i ett flervalsområde. |
| [getSelectCells()](#getSelectCells--) | Hämtar samlingen av markerade celler. |
| [getSessionStorePath()](#getSessionStorePath--) | Hämtar sökvägen för sessionscachelagring när sessionsläget är File eller ViewState, etc: gridweb.SessionStorePath="c:/mytempdir/session"; då lagras sessionsdata i c:/mytempdir/session |
| [getSettings()](#getSettings--) | Representerar arbetsbokens inställningar. |
| [getShowAddButton()](#getShowAddButton--) | Hämtar om knappen för att lägga till kalkylblad ska visas. |
| [getShowBottomBar()](#getShowBottomBar--) | Anger om kommandoraden (inkluderar kommandorad och flikrad) ska visas längst ner i kontrollen. |
| [getShowCellEditBox()](#getShowCellEditBox--) | Om Gridweb visar verktygsfältet för redigeringsruta som i MS‑EXCEL. Om aktiverat visas en redigeringsruta för den aktuella cellen i Gridweb. |
| [getShowCommandBarAtTop()](#getShowCommandBarAtTop--) | Anger om kommandoraden (inkluderar kommandorad och flikrad) ska visas högst upp i kontrollen. |
| [getShowContextMenu()](#getShowContextMenu--) | Hämtar om snabbmenyn ska visas. Standardvärdet är true. |
| [getShowDefaultGridLine()](#getShowDefaultGridLine--) | Hämtar om standardrutnätslinjerna för cellerna ska visas. |
| [getShowHeaderBar()](#getShowHeaderBar--) | Hämtar om rubrikfältet ska visas |
| [getShowLoading()](#getShowLoading--) | Anger om en laddningsdialogruta ska visas under postback till servern. |
| [getShowLoadingPosition()](#getShowLoadingPosition--) | Anger vänster- och topposition (i px) för att visa laddningsdialogrutan under postback till servern, osv. 100,200 betyder att laddningsdialogrutans vänster- och topposition är 100 px, 200 px. |
| [getShowSaveButton()](#getShowSaveButton--) | Hämtar om spara‑knappen ska visas. |
| [getShowSubmitButton()](#getShowSubmitButton--) | Hämtar om skicka‑knappen ska visas. |
| [getShowTabBar()](#getShowTabBar--) | Hämtar om flikfältet ska visas. |
| [getShowTabNavigation()](#getShowTabNavigation--) | Hämtar om fliknavigationsknappen visas, standardvärdet är true. |
| [getShowUndoButton()](#getShowUndoButton--) | Hämtar om ångra‑knappen ska visas. |
| [getSpanWrap()](#getSpanWrap--) | Anger om innehållet ska radbrytas i cellspannet, standardvärdet är true. |
| [getTabIndex()](#getTabIndex--) | Hämtar TabIndex i WebControl |
| [getTabStyle()](#getTabStyle--) | Hämtar stilen för flikfältet. |
| [getToolTip()](#getToolTip--) | Hämtar ToolTip i WebControl |
| [getUseClientPageHeight()](#getUseClientPageHeight--) | Hämtar om GridWeb använder klientens sidhöjd som kontrollhöjd, lämpligt när Height="100%" är satt, standardvärdet är false. |
| [getVersion()](#getVersion--) | Hämta utgivningsversionen. |
| [getViewPanelScrollLeft()](#getViewPanelScrollLeft--) | Hämtar positionen för rullningslisten i gridens visningspanel. |
| [getViewPanelScrollTop()](#getViewPanelScrollTop--) | Hämtar positionen för rullningslisten i gridens visningspanel. |
| [getViewTableStyle()](#getViewTableStyle--) | Hämtar stilen för datavisningspanelen. |
| [getWidth()](#getWidth--) | Hämtar bredden (System.Web.UI.WebControl.Unit) för kontrollen. |
| [getWorkSheets()](#getWorkSheets--) | Hämtar samlingen av arbetsblad. |
| [getXhtmlMode()](#getXhtmlMode--) | Hämtar om XHTML‑stil ska användas, standardvärdet är true. |
| [hashCode()](#hashCode--) |  |
| [importExcelFile(InputStream stream)](#importExcelFile-java.io.InputStream-) | Importerar från en Excel‑filström, inklusive filström från disk eller minnesström. |
| [importExcelFile(InputStream stream, String passwordtoOpen)](#importExcelFile-java.io.InputStream-java.lang.String-) | Importerar från en Excel‑filström, inklusive filström från disk eller minnesström. |
| [importExcelFile(String fileName)](#importExcelFile-java.lang.String-) | Importerar från en Excel‑fil. |
| [importExcelFile(String fileName, String passwordtoOpen)](#importExcelFile-java.lang.String-java.lang.String-) | Importerar från en Excel‑fil. |
| [isCalculateFormula()](#isCalculateFormula--) | Hämtar om formeln ska beräknas efter att cellvärdet ändras eller efter import av fil. |
| [loadCSVFile(InputStream stream)](#loadCSVFile-java.io.InputStream-) | Läser in data från en CSV‑filström. |
| [loadCSVFile(String fileName)](#loadCSVFile-java.lang.String-) | Läser in data från en CSV‑fil. |
| [loadHTMLFile(InputStream stream)](#loadHTMLFile-java.io.InputStream-) | Läser in data från en HTML‑filström. |
| [loadHTMLFile(String fileName)](#loadHTMLFile-java.lang.String-) | Läser in data från en HTML‑fil. |
| [loadSpreadSheetMLFile(InputStream stream)](#loadSpreadSheetMLFile-java.io.InputStream-) | Läser in data från en SpreadSheetML‑filström. |
| [loadSpreadSheetMLFile(String fileName)](#loadSpreadSheetMLFile-java.lang.String-) | Läser in data från en SpreadSheetML‑fil. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshChartShape()](#refreshChartShape--) | uppdatera alla diagrambilder för det aktiva kalkylbladet. |
| [saveCSVFile(OutputStream stream)](#saveCSVFile-java.io.OutputStream-) | Sparar data till en CSV-filström. |
| [saveCSVFile(String targetFile)](#saveCSVFile-java.lang.String-) | Sparar data till en CSV-fil. |
| [saveCustomStyleFile(String fileName)](#saveCustomStyleFile-java.lang.String-) | Sparar aktuell stildata för kontrollen till en XML-fil. |
| [saveHTMLFile(OutputStream stream)](#saveHTMLFile-java.io.OutputStream-) | Sparar data till en HTML-filström. |
| [saveHTMLFile(String targetFile)](#saveHTMLFile-java.lang.String-) | Sparar data till en HTML-fil. |
| [saveSpreadSheetMLFile(OutputStream stream)](#saveSpreadSheetMLFile-java.io.OutputStream-) | Sparar data till en SpreadSheetML-filström. |
| [saveSpreadSheetMLFile(String targetFile)](#saveSpreadSheetMLFile-java.lang.String-) | Sparar data till en SpreadSheetML-fil. |
| [saveToExcelFile(OutputStream stream)](#saveToExcelFile-java.io.OutputStream-) | Sparar arbetsbladen till en Excel-fil. |
| [saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)](#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-) | Sparar arbetsbladen till en Excel-fil. |
| [saveToExcelFile(OutputStream stream, int format)](#saveToExcelFile-java.io.OutputStream-int-) | Sparar arbetsbladen till en Excel-fil. |
| [saveToExcelFile(String targetFile)](#saveToExcelFile-java.lang.String-) | Sparar arbetsbladen till en Excel-fil i Excel 2003-format. |
| [saveToExcelFile(String targetFile, GridSaveOptions saveOptions)](#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-) | Sparar arbetsbladen till en Excel-fil. |
| [saveToExcelFile(String targetFile, int format)](#saveToExcelFile-java.lang.String-int-) | Sparar arbetsbladen till en Excel-fil. |
| [setACWClientPath(String value)](#setACWClientPath-java.lang.String-) | Ställer in webbvägen för skript-/bildfiler för kontrollen. |
| [setACWLanguageFileUrl(String value)](#setACWLanguageFileUrl-java.lang.String-) | Ställer in webbadressen för språkfilen för kontrollen. |
| [setActiveCell(GridCell value)](#setActiveCell-com.aspose.gridweb.GridCell-) | Ställer in den aktiva cellen i det aktuella bladet. |
| [setActiveCellBgColor(Color value)](#setActiveCellBgColor-com.aspose.gridweb.Color-) | Anger bakgrundsfärgen för den aktiva cellen. |
| [setActiveCellColor(Color value)](#setActiveCellColor-com.aspose.gridweb.Color-) | Anger färgen för den aktiva cellen. |
| [setActiveHeaderBgColor(Color value)](#setActiveHeaderBgColor-com.aspose.gridweb.Color-) | Anger bakgrundsfärgen för den aktiva rad‑/kolumnrubriken. |
| [setActiveHeaderColor(Color value)](#setActiveHeaderColor-com.aspose.gridweb.Color-) | Anger färgen för den aktiva rad‑/kolumnrubriken. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Ställer in index för det aktiva bladet. |
| [setActiveTabStyle(GridTableItemStyle value)](#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Anger stilen för den aktiva fliken. |
| [setAutoRefreshChart(boolean value)](#setAutoRefreshChart-boolean-) | Ställer in om diagrambilden uppdateras när cellvärdet uppdateras. standardvärdet är true |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Ställer in BackColor i WebControl |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Ställer in BorderColor i WebControl |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Ställer in BorderStyle i WebControl |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Ställer in BorderWidth i WebControl |
| [setBottomTableStyle(GridTableStyle value)](#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-) | Ställer in stilen för kontrollens nedre verktygsfält. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Ställer in om formeln ska beräknas efter att cellvärdet ändras eller efter import av fil. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Ställer in CssClass i WebControl |
| [setCurrentPageIndex(int value)](#setCurrentPageIndex-int-) | Ställer in index för aktuell sida i pagineringsläge. |
| [setCustomCalculationEngine(GridAbstractCalculationEngine value)](#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-) | Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells. |
| [setCustomStyle(InputStream stream)](#setCustomStyle-java.io.InputStream-) | ställer in den anpassade stilfilen från en ström, inklusive filströmmar från disk eller minne. |
| [setCustomStyleFileName(String value)](#setCustomStyleFileName-java.lang.String-) | Ställer in namn på den anpassade stilfilen. |
| [setDPI(double value)](#setDPI-double-) | Hämtar /Ställer in DPI för maskinen. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Ställer in kontrollens standardteckensnittsnamn. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | Ställer in kontrollens standardteckenstorlek. |
| [setDefaultGridLineColor(Color value)](#setDefaultGridLineColor-com.aspose.gridweb.Color-) | Ställer in standardfärgen för rutnätslinjer. |
| [setDisplayCellTip(boolean value)](#setDisplayCellTip-boolean-) | Ställer in om tips ska visas. standardvärdet är true. |
| [setEditMode(boolean value)](#setEditMode-boolean-) | Ställer in kontrollens redigeringsläge. |
| [setEnableAJAX(boolean value)](#setEnableAJAX-boolean-) | Ställer in om AJAX-anrop ska användas. standardvärdet är true. |
| [setEnableAsync(boolean value)](#setEnableAsync-boolean-) | Ställer in om laddningsceller data ska hanteras asynkront, föreslås att tillämpas för ett blad med mer än 10000 celler. |
| [setEnableClientColumnOperations(boolean value)](#setEnableClientColumnOperations-boolean-) | Ställer in om kolumnoperationer på klientsidan ska aktiveras. |
| [setEnableClientFreeze(boolean value)](#setEnableClientFreeze-boolean-) | Ställer in om frysningsoperationer på klientsidan ska aktiveras. |
| [setEnableClientMergeOperations(boolean value)](#setEnableClientMergeOperations-boolean-) | Ställer in om sammanslagningsoperationer på klientsidan ska aktiveras. |
| [setEnableClientResizeColumnRow(boolean value)](#setEnableClientResizeColumnRow-boolean-) | Ställer in om ändring av kolumn- och radstorlek på klientsidan ska aktiveras. |
| [setEnableClientRowOperations(boolean value)](#setEnableClientRowOperations-boolean-) | Ställer in om radoperationer på klientsidan ska aktiveras. |
| [setEnableDoubleClickEvent(boolean value)](#setEnableDoubleClickEvent-boolean-) | Ställer in om dubbelklickshändelse på kundsidan ska aktiveras. |
| [setEnableMetalLightEffect(boolean value)](#setEnableMetalLightEffect-boolean-) | Ställer in om metallljuseffekt ska tillämpas. |
| [setEnablePaging(boolean value)](#setEnablePaging-boolean-) | Ställer in om kontrollens sidindelningsläge ska aktiveras. |
| [setEnableStyleDialogbox(boolean value)](#setEnableStyleDialogbox-boolean-) | Ställer in om stil‑dialogrutan på klientsidan ska aktiveras. |
| [setEnabled(boolean value)](#setEnabled-boolean-) | Ställer in Enabled i WebControl |
| [setFilteredPaging(boolean value)](#setFilteredPaging-boolean-) | Ställer in om sidindelning ska aktiveras efter att data filtrerats, påverkar när EnablePaging är sant. |
| [setFontFolder(String fontFolder, boolean recursive)](#setFontFolder-java.lang.String-boolean-) | Ställer in teckensnittsmappen |
| [setFontFolders(String[] fontFolders, boolean recursive)](#setFontFolders-java.lang.String---boolean-) | Ställer in teckensnittsmapparna |
| [setForceValidation(boolean value)](#setForceValidation-boolean-) | Ställer in om validering på kundsidan ska tvingas. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Ställer in ForeColor i WebControl |
| [setFrameTableStyle(GridTableStyle value)](#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-) | Ställer in ramstilen för kontrollen. |
| [setGoonDefaultSaveOperation(boolean value)](#setGoonDefaultSaveOperation-boolean-) | Ställer in om GridWeb ska utföra standard‑sparoperation, standardvärdet är sant. |
| [setHeaderBarHeight(Unit value)](#setHeaderBarHeight-com.aspose.gridweb.Unit-) | Ställer in höjden (System.Web.UI.WebControl.Unit) för kontrollens övre rubrikrad. |
| [setHeaderBarStyle(GridTableItemStyle value)](#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-) | Ställer in rubrikradens stil. |
| [setHeaderBarTableStyle(GridTableStyle value)](#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-) | Ställer in rubrikradens stil för kontrollen. |
| [setHeaderBarWidth(Unit value)](#setHeaderBarWidth-com.aspose.gridweb.Unit-) | Ställer in bredden (System.Web.UI.WebControl.Unit) för kontrollens vänstra rubrikrad. |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Ställer in höjden (System.Web.UI.WebControl.Unit) för kontrollen. |
| [setIgnoreStyleWithNoData(boolean value)](#setIgnoreStyleWithNoData-boolean-) | Ställer in om GridWeb ignorerar visning av rader eller kolumner som inte innehåller cellvärden men ändå är formaterade. |
| [setLoadOptions(GridLoadOptions value)](#setLoadOptions-com.aspose.gridweb.GridLoadOptions-) | Representerar laddningsalternativen för GridWeb. |
| [setMaxColumn(int value)](#setMaxColumn-int-) | Ställer in det maximala visningskolumnindexet (nollbaserat) för webblådan. |
| [setMaxRow(int value)](#setMaxRow-int-) | Ställer in det maximala visningsradindexet (nollbaserat) för webblådan. |
| [setMessage(String value)](#setMessage-java.lang.String-) | Ställer in meddelandet för rutnätet. |
| [setMinColumn(int value)](#setMinColumn-int-) | Ställer in det minsta visningskolumnindexet (nollbaserat) för webblådan. |
| [setMinRow(int value)](#setMinRow-int-) | Ställer in det minsta visningsradindexet (nollbaserat) för webblådan. |
| [setNeedRenderGroupRows(boolean value)](#setNeedRenderGroupRows-boolean-) | Ställer in om grupprader ska visas. |
| [setNoHScroll(boolean value)](#setNoHScroll-boolean-) | Ställer in ett värde som indikerar om den horisontella rullningslisten är dold. |
| [setNoScroll(boolean value)](#setNoScroll-boolean-) | Ställer in om rullningslisten ska visas. |
| [setNoVScroll(boolean value)](#setNoVScroll-boolean-) | Ställer in ett värde som indikerar om den vertikala rullningslisten är dold. |
| [setOnAjaxCallFinishedClientFunction(String value)](#setOnAjaxCallFinishedClientFunction-java.lang.String-) | Ställer in klient‑sidans funktionsnamn som ska anropas när ajax‑anropet är slutfört. |
| [setOnCellErrorClientFunction(String value)](#setOnCellErrorClientFunction-java.lang.String-) | Ställer in klient‑sidans funktionsnamn som ska anropas när en cells validering misslyckas. |
| [setOnCellSelectedAjaxCallBackClientFunction(String value)](#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-) | Ställer in klient‑sidans funktion som ska anropas när en cell har markerats. |
| [setOnCellSelectedClientFunction(String value)](#setOnCellSelectedClientFunction-java.lang.String-) | Ställer in klient‑sidans funktion som ska anropas när en cell har markerats. |
| [setOnCellUnselectedClientFunction(String value)](#setOnCellUnselectedClientFunction-java.lang.String-) | Ställer in klient‑sidans funktion som ska anropas när en cell avmarkerats. |
| [setOnCellUpdatedClientFunction(String value)](#setOnCellUpdatedClientFunction-java.lang.String-) | Ställer in klient‑sidans funktionsnamn som ska anropas när en cells värde har uppdaterats. |
| [setOnContextMenuShowClientFunction(String value)](#setOnContextMenuShowClientFunction-java.lang.String-) | Ställer in klient‑sidans funktion som ska anropas när snabbmenyn visas. |
| [setOnDoubleClickCellClientFunction(String value)](#setOnDoubleClickCellClientFunction-java.lang.String-) | Ställer in klient‑sidans funktion som ska anropas när en cell dubbelklickas. |
| [setOnDoubleClickRowClientFunction(String value)](#setOnDoubleClickRowClientFunction-java.lang.String-) | Ställer in klient‑sidans funktion som ska anropas när en rad dubbelklickas. |
| [setOnGridInitClientFunction(String value)](#setOnGridInitClientFunction-java.lang.String-) | Ställer in klient‑sidans funktionsnamn som ska anropas när rutnätet initieras. |
| [setOnPageChangeClientFunction(String value)](#setOnPageChangeClientFunction-java.lang.String-) | Ställer in klient‑sidans funktion som ska anropas efter sidindexändring. Gäller endast när EnablePaging är sant. |
| [setOnPageSubmitClientFunction(String value)](#setOnPageSubmitClientFunction-java.lang.String-) | Ställer in klientfunktionen som ska anropas innan sidan skickas från klienten. |
| [setOnShapeSelectedClientFunction(String value)](#setOnShapeSelectedClientFunction-java.lang.String-) | Ställer in klient‑sidans funktion som ska anropas när en form har markerats. |
| [setOnSubmitClientFunction(String value)](#setOnSubmitClientFunction-java.lang.String-) | Ställer in klientfunktionen som ska anropas innan kontrollen skickas från klienten. |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | Ställer in om endast rader vars höjd inte är anpassad ska anpassas, standardvärdet är falskt. |
| [setPageSize(int value)](#setPageSize-int-) | Ställer in sidstorleken i pagineringsläge. |
| [setPictureCachePath(String value)](#setPictureCachePath-java.lang.String-) | Ställer in bildlagringssökvägen för arbetsboken, alla former och bilder lagras i den här katalogen, standardsökvägen är acwcache under den aktuella applikationens baskatalog. Användare måste implementera en schemalagd tjänst för att rensa filer som har gått utanför sessionstiden. |
| [setPresetStyle(int value)](#setPresetStyle-int-) | Ställer in den förinställda stilen. |
| [setRefreshValidation(boolean value)](#setRefreshValidation-boolean-) | Ställer in om valideringsvärdet ska uppdateras efter att cellvärdet ändras. |
| [setRenderHiddenRow(boolean value)](#setRenderHiddenRow-boolean-) | Ställer in om den dolda raden ska renderas i GridControl, standardvärdet är falskt. |
| [setRowHeightForCSV(double value)](#setRowHeightForCSV-double-) | Ställer in radens höjd i punkter för CSV‑fil, standardvärdet är 14,5. |
| [setScrollBarArrowColor(Color value)](#setScrollBarArrowColor-com.aspose.gridweb.Color-) | Anger färgen på rullningslistens pilknapp. |
| [setScrollBarBaseColor(Color value)](#setScrollBarBaseColor-com.aspose.gridweb.Color-) | Anger färgen på kontrollens rullningslist. |
| [setSelectCellBgColor(Color value)](#setSelectCellBgColor-com.aspose.gridweb.Color-) | Anger bakgrundsfärgen för de markerade cellerna i ett flervalsområde. |
| [setSelectCellColor(Color value)](#setSelectCellColor-com.aspose.gridweb.Color-) | Anger färgen på de markerade cellerna i ett flervalsområde. |
| [setSessionStorePath(String value)](#setSessionStorePath-java.lang.String-) | Ställer in sökvägen för sessionscachelagring när sessionsläget är File eller ViewState, t.ex.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; då lagras sessionsdata i c:/mytempdir/session. |
| [setSettings(GridWorkbookSettings value)](#setSettings-com.aspose.gridweb.GridWorkbookSettings-) | Representerar arbetsbokens inställningar. |
| [setShowAddButton(boolean value)](#setShowAddButton-boolean-) | Ställer in om knappen för att lägga till kalkylblad ska visas. |
| [setShowBottomBar(boolean value)](#setShowBottomBar-boolean-) | Anger om kommandoraden (inkluderar kommandorad och flikrad) ska visas längst ner i kontrollen. |
| [setShowCellEditBox(boolean value)](#setShowCellEditBox-boolean-) | Om Gridweb visar verktygsfältet för redigeringsruta som i MS‑EXCEL. Om aktiverat visas en redigeringsruta för den aktuella cellen i Gridweb. |
| [setShowCommandBarAtTop(boolean value)](#setShowCommandBarAtTop-boolean-) | Anger om kommandoraden (inkluderar kommandorad och flikrad) ska visas högst upp i kontrollen. |
| [setShowContextMenu(boolean value)](#setShowContextMenu-boolean-) | Ställer in om snabbmenyn ska visas. standardvärdet är true. |
| [setShowDefaultGridLine(boolean value)](#setShowDefaultGridLine-boolean-) | Ställer in om cellernas standardrutlinjer ska visas. |
| [setShowHeaderBar(boolean value)](#setShowHeaderBar-boolean-) | Ställer in om rubrikfältet ska visas |
| [setShowLoading(boolean value)](#setShowLoading-boolean-) | Anger om en laddningsdialogruta ska visas under postback till servern. |
| [setShowLoadingPosition(String value)](#setShowLoadingPosition-java.lang.String-) | Anger vänster- och topposition (i px) för att visa laddningsdialogrutan under postback till servern, osv. 100,200 betyder att laddningsdialogrutans vänster- och topposition är 100 px, 200 px. |
| [setShowSaveButton(boolean value)](#setShowSaveButton-boolean-) | Ställer in om spara-knappen ska visas. |
| [setShowSubmitButton(boolean value)](#setShowSubmitButton-boolean-) | Ställer in om skicka-knappen ska visas. |
| [setShowTabBar(boolean value)](#setShowTabBar-boolean-) | Ställer in om flikfältet ska visas. |
| [setShowTabNavigation(boolean value)](#setShowTabNavigation-boolean-) | Ställer in om fliknavigationsknappen ska visas, standardvärdet är true. |
| [setShowUndoButton(boolean value)](#setShowUndoButton-boolean-) | Ställer in om ångra-knappen ska visas. |
| [setSpanWrap(boolean value)](#setSpanWrap-boolean-) | Anger om innehållet ska radbrytas i cellspannet, standardvärdet är true. |
| [setTabIndex(short value)](#setTabIndex-short-) | Ställer in TabIndex i WebControl |
| [setTabStyle(GridTableItemStyle value)](#setTabStyle-com.aspose.gridweb.GridTableItemStyle-) | Ställer in stilen för flikfältet. |
| [setToolTip(String value)](#setToolTip-java.lang.String-) | Ställer in ToolTip i WebControl |
| [setUseClientPageHeight(boolean value)](#setUseClientPageHeight-boolean-) | Ställer in om GridWeb ska använda klientens sidhöjd som kontrollhöjd, lämpligt när Height="100%" är satt, standardvärdet är false |
| [setViewPanelScrollLeft(String value)](#setViewPanelScrollLeft-java.lang.String-) | Ställer in positionen för rullningslisten i rutnätets visningspanel. |
| [setViewPanelScrollTop(String value)](#setViewPanelScrollTop-java.lang.String-) | Ställer in positionen för rullningslisten i rutnätets visningspanel. |
| [setViewTableStyle(GridTableStyle value)](#setViewTableStyle-com.aspose.gridweb.GridTableStyle-) | Ställer in stilen för datavisningspanelen. |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Ställer in bredden (System.Web.UI.WebControl.Unit) för kontrollen. |
| [setXhtmlMode(boolean value)](#setXhtmlMode-boolean-) | Ställer in om XHTML-stil ska användas, standardvärdet är true. |
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


Uppstår efter att kolumnen filtrerats.

### AjaxCallFinished {#AjaxCallFinished}
```
public WorkbookEventHandler AjaxCallFinished
```


Utlöses när AJAX-uppdateringen av kontrollen är klar (EnableAJAX ska vara satt till true).

### BeforeColumnFilter {#BeforeColumnFilter}
```
public RowColumnEventHandler BeforeColumnFilter
```


Uppstår innan kolumnen ska filtreras.

### CellClickOnAjax {#CellClickOnAjax}
```
public CellEventStringHandler CellClickOnAjax
```


Uppstår när cellen klickas, och ett ajaxcallback behövs för denna händelse.

### CellClientUpdate {#CellClientUpdate}
```
public CellEventHandler CellClientUpdate
```


Inträffar när en klientcelluppdatering sker. När denna händelse utlöses innehåller dess parameter e.Argument kommandots namn.

### CellCommand {#CellCommand}
```
public CellEventHandler CellCommand
```


Inträffar när en cells kommandolänk klickas. När denna händelse utlöses innehåller dess parameter e.Argument kommandots namn.

### CellDoubleClick {#CellDoubleClick}
```
public CellEventHandler CellDoubleClick
```


Uppstår när cellen dubbelklickas.

### CellModifiedOnAjax {#CellModifiedOnAjax}
```
public CellEventHandler CellModifiedOnAjax
```


Uppstår när cellen ändras i ajaxcall.

### ColumnDeleted {#ColumnDeleted}
```
public RowColumnEventHandler ColumnDeleted
```


Uppstår när användaren tar bort en kolumn från den klient‑baserade menyn.

### ColumnDeleting {#ColumnDeleting}
```
public RowColumnEventHandler ColumnDeleting
```


Inträffar när användaren försöker ta bort en kolumn från den klientbaserade menyn. Du kan hantera denna händelse och sätta avbryt‑parametern till True för att avbryta borttagningsoperationen.

### ColumnDoubleClick {#ColumnDoubleClick}
```
public RowColumnEventHandler ColumnDoubleClick
```


Uppstår när kolumnrubriken dubbelklickas.

### ColumnInserted {#ColumnInserted}
```
public RowColumnEventHandler ColumnInserted
```


Uppstår när användaren infogar en kolumn från den klientbaserade menyn.

### CustomCommand {#CustomCommand}
```
public CustomCommandEventHandler CustomCommand
```


Uppstår när användaren klickar på en anpassad kommandoknapp.

### LoadCustomData {#LoadCustomData}
```
public WorkbookEventHandler LoadCustomData
```


Utlöses när kontrollens SessionMode är satt till Custom och behöver ladda bladdata. Du kan hantera denna händelse i Custom Session‑läge för att ladda bladdata från fil eller databas.

### PageIndexChanged {#PageIndexChanged}
```
public WorkbookEventHandler PageIndexChanged
```


Uppstår när kontrollens bladsidindex har ändrats.

### RowDeleted {#RowDeleted}
```
public RowColumnEventHandler RowDeleted
```


Uppstår när användaren har tagit bort en rad från den klientbaserade menyn.

### RowDeleting {#RowDeleting}
```
public RowColumnEventHandler RowDeleting
```


Inträffar när användaren försöker ta bort en rad från den klientbaserade menyn. Du kan hantera denna händelse och kasta ett RejectDeleteException‑undantag för att avbryta borttagningsoperationen.

### RowDoubleClick {#RowDoubleClick}
```
public RowColumnEventHandler RowDoubleClick
```


Uppstår när radrubriken dubbelklickas.

### RowInserted {#RowInserted}
```
public RowColumnEventHandler RowInserted
```


Uppstår när användaren infogar en rad från den klientbaserade menyn.

### SaveCommand {#SaveCommand}
```
public WorkbookEventHandler SaveCommand
```


Uppstår när "spara"-knappen klickas.

### SheetAdded {#SheetAdded}
```
public SheetEventHandler SheetAdded
```


Uppstår när användaren lägger till ett arbetsblad från verktygsfältets meny.

### SheetTabClick {#SheetTabClick}
```
public WorkbookEventHandler SheetTabClick
```


Uppstår när bladfliken klickas.

### SubmitCommand {#SubmitCommand}
```
public WorkbookEventHandler SubmitCommand
```


Uppstår när "skicka"-knappen klickas.

### UndoCommand {#UndoCommand}
```
public WorkbookEventHandler UndoCommand
```


Uppstår när "ångra"-knappen klickas.

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Beräknar resultatet av formler.

### createChildControls() {#createChildControls--}
```
public void createChildControls()
```


implementera CreateChildControls från WebControl, endast för internt bruk.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getACWClientPath() {#getACWClientPath--}
```
public String getACWClientPath()
```


Hämtar webbvägen för skript-/bildfilerna för kontrollen. Till exempel: "http://localhost/acw\_client". Du kan också sätta detta värde i web.config‑filen. Lägg till detta avsnitt i `<configuration>`‑sektionen:
`<appSettings>`
`<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />`
`</appSettings>`


**Returns:**
java.lang.String
### getACWLanguageFileUrl() {#getACWLanguageFileUrl--}
```
public String getACWLanguageFileUrl()
```


Hämtar webbadressen för språkfilen för kontrollen. Till exempel: "/acw\_client/lang\_en.js".
Som standard används en inbyggd engelsk fil.


**Returns:**
java.lang.String
### getActiveCell() {#getActiveCell--}
```
public GridCell getActiveCell()
```


Hämtar den aktiva cellen i det aktuella bladet. Ändrad till skrivbar sedan version 1.9.0.1.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getActiveCellBgColor() {#getActiveCellBgColor--}
```
public Color getActiveCellBgColor()
```


Anger bakgrundsfärgen för den aktiva cellen.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveCellColor() {#getActiveCellColor--}
```
public Color getActiveCellColor()
```


Anger färgen för den aktiva cellen.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderBgColor() {#getActiveHeaderBgColor--}
```
public Color getActiveHeaderBgColor()
```


Anger bakgrundsfärgen för den aktiva rad‑/kolumnrubriken.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveHeaderColor() {#getActiveHeaderColor--}
```
public Color getActiveHeaderColor()
```


Anger färgen för den aktiva rad‑/kolumnrubriken.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getActiveSheet() {#getActiveSheet--}
```
public GridWorksheet getActiveSheet()
```


Hämtar det aktiva bladet

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Hämtar indexet för det aktiva bladet. Lika med WebWorksheets.ActiveSheetIndex.

**Returns:**
int
### getActiveTabStyle() {#getActiveTabStyle--}
```
public GridTableItemStyle getActiveTabStyle()
```


Anger stilen för den aktiva fliken.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getAutoRefreshChart() {#getAutoRefreshChart--}
```
public boolean getAutoRefreshChart()
```


Hämtar om diagrambilden uppdateras medan cellvärdet uppdateras. standardvärdet är true

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Hämtar BackColor i WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Hämtar BorderColor i WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Hämtar BorderStyle i WebControl

Se [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Hämtar BorderWidth i WebControl

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomTableStyle() {#getBottomTableStyle--}
```
public GridTableStyle getBottomTableStyle()
```


Hämtar stilen för kontrollens nedre stapel.

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


Hämtar CssClass i WebControl

**Returns:**
java.lang.String
### getCurrentPageIndex() {#getCurrentPageIndex--}
```
public int getCurrentPageIndex()
```


Hämtar det aktuella sidindexet i pagineringsläge.

**Remarks**

När den är i sidindelningsläge visar kontrollen PageSize rader data en gång, och visar sidvalskontrollen i flikfältet.

**Returns:**
int
### getCustomCalculationEngine() {#getCustomCalculationEngine--}
```
public GridAbstractCalculationEngine getCustomCalculationEngine()
```


Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells.

**Returns:**
[GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine)
### getCustomCommandButtons() {#getCustomCommandButtons--}
```
public CustomCommandButtonCollection getCustomCommandButtons()
```


Hämtar den anpassade samlingen av kommandoknappar

**Returns:**
[CustomCommandButtonCollection](../../com.aspose.gridweb/customcommandbuttoncollection)
### getCustomStyleFileName() {#getCustomStyleFileName--}
```
public String getCustomStyleFileName()
```


Hämtar det anpassade stilfilnamnet.

**Remarks**

Den anpassade stilfilen är en XML-fil. När du anger filnamnet laddas filen omedelbart. Här är innehållet i den "standard förinställda stilen" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

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


Hämtar /Ställer in DPI för maskinen.

**Remarks**

**Returns:**
double
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Hämtar kontrollens standardteckensnittsnamn.

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


Hämtar kontrollens standardteckenstorlek.

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


Hämtar standardrutnätslinjens färg.

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


Hämtar om tips ska visas. standardvärdet är true.

**Returns:**
boolean
### getEditMode() {#getEditMode--}
```
public boolean getEditMode()
```


Hämtar kontrollens redigeringsläge.

**Remarks**

När den är satt till true, är kontrollens celler redigerbara, och ikonerna "save" och "undo" visas. När den är satt till false, är kontrollens celler skrivskyddade, och ikonerna "save" och "undo" visas inte.

**Returns:**
boolean
### getEnableAJAX() {#getEnableAJAX--}
```
public boolean getEnableAJAX()
```


Hämtar om AJAX-anrop ska användas. standardvärdet är true.

**Returns:**
boolean
### getEnableAsync() {#getEnableAsync--}
```
public boolean getEnableAsync()
```


Hämtar om celldata laddas asynkront, föreslås för ett blad med mer än 10000 celler.

**Returns:**
boolean
### getEnableClientColumnOperations() {#getEnableClientColumnOperations--}
```
public boolean getEnableClientColumnOperations()
```


Hämtar om kolumnoperationer på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren använda högerklicksmenyn för att lägga till/ta bort kolumner.

**Returns:**
boolean
### getEnableClientFreeze() {#getEnableClientFreeze--}
```
public boolean getEnableClientFreeze()
```


Hämtar om frysningsoperationer på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren använda högerklicksmenyn för att frysa/töja paneler.

**Returns:**
boolean
### getEnableClientMergeOperations() {#getEnableClientMergeOperations--}
```
public boolean getEnableClientMergeOperations()
```


Hämtar om sammanslagningsoperationer på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren använda högerklicksmenyn för att slå ihop/ta isär celler.

**Returns:**
boolean
### getEnableClientResizeColumnRow() {#getEnableClientResizeColumnRow--}
```
public boolean getEnableClientResizeColumnRow()
```


Hämtar om ändring av kolumn- och radstorlek på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren ändra storlek på kolumnen och raden på klientsidan.

**Returns:**
boolean
### getEnableClientRowOperations() {#getEnableClientRowOperations--}
```
public boolean getEnableClientRowOperations()
```


Hämtar om radoperationer på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren använda högerklicksmenyn för att lägga till/ta bort rader.

**Returns:**
boolean
### getEnableDoubleClickEvent() {#getEnableDoubleClickEvent--}
```
public boolean getEnableDoubleClickEvent()
```


Hämtar om kundsidans dubbelklickshändelse ska aktiveras.

**Remarks**

När den är satt till true kommer kontrollen att ta emot dubbelklickshändelser på kundsidan och du kan hantera dessa händelser på serversidan. Annars kommer kontrollen att ignorera alla dubbelklickshändelser.

**Returns:**
boolean
### getEnableMetalLightEffect() {#getEnableMetalLightEffect--}
```
public boolean getEnableMetalLightEffect()
```


Hämtar om metallljuseffekt ska tillämpas.

**Returns:**
boolean
### getEnablePaging() {#getEnablePaging--}
```
public boolean getEnablePaging()
```


Hämtar om kontrollens pagineringsläge ska aktiveras.

**Remarks**

När den är satt till true kommer kontrollen att visa PageSize rader med data på en gång, och visa sidvalskontrollen i flikfältet.

**Returns:**
boolean
### getEnableStyleDialogbox() {#getEnableStyleDialogbox--}
```
public boolean getEnableStyleDialogbox()
```


Hämtar om stil‑dialogrutan på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren använda stil-dialogrutan för att sätta en cells stil genom att välja "Format Cell..." i popup-menyn.

**Returns:**
boolean
### getEnabled() {#getEnabled--}
```
public boolean getEnabled()
```


Hämtar Enabled i WebControl

**Returns:**
boolean
### getFilteredPaging() {#getFilteredPaging--}
```
public boolean getFilteredPaging()
```


Hämtar om paginering ska aktiveras efter att data filtrerats, träder i kraft när EnablePaging är true.

**Remarks**

När den är satt till true kommer kontrollen att paginera baserat på filtrerade data, standardvärdet är false.

**Returns:**
boolean
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Hämtar Font i WebControl

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForceValidation() {#getForceValidation--}
```
public boolean getForceValidation()
```


Hämtar om kundsidans validering ska tvingas.

**Remarks**

När den är satt till true kommer data inte att skickas till servern förrän alla inmatningsfält är giltiga.

**Returns:**
boolean
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Hämtar ForeColor i WebControl

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getFrameTableStyle() {#getFrameTableStyle--}
```
public GridTableStyle getFrameTableStyle()
```


Hämtar ramstilen för kontrollen.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getGoonDefaultSaveOperation() {#getGoonDefaultSaveOperation--}
```
public boolean getGoonDefaultSaveOperation()
```


Hämtar om GridWeb kommer att utföra standard‑sparåtgärden, standardvärdet är true.

**Returns:**
boolean
### getHeaderBarHeight() {#getHeaderBarHeight--}
```
public Unit getHeaderBarHeight()
```


Hämtar höjden( System.Web.UI.WebControl.Unit ) för kontrollens översta rubrikfält.

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


Hämtar rubrikfältets stil.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getHeaderBarTableStyle() {#getHeaderBarTableStyle--}
```
public GridTableStyle getHeaderBarTableStyle()
```


Hämtar rubrikfältets stil för kontrollen.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getHeaderBarWidth() {#getHeaderBarWidth--}
```
public Unit getHeaderBarWidth()
```


Hämtar bredden( System.Web.UI.WebControl.Unit ) för kontrollens vänstra rubrikfält.

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


Hämtar höjden( System.Web.UI.WebControl.Unit ) för kontrollen.

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


Hämtar om GridWeb ignorerar att visa rader eller kolumner som inte innehåller cellvärden men ändå är stylade. Om den är satt till true blir prestandan bättre. Standardvärdet är false, vilket betyder att om den sista på varandra följande raden/kolumnen saknar cellvärden men är stylad, kommer vi fortfarande att visa dem. Detta alternativ är endast giltigt när EnableAsync är false. Detta alternativ har ingen effekt när EnableAsync är true, vilket betyder att GridWeb kommer att visa alla rader/kolumner med stil.

**Returns:**
boolean
### getLoadOptions() {#getLoadOptions--}
```
public GridLoadOptions getLoadOptions()
```


Representerar laddningsalternativen för GridWeb.

**Returns:**
[GridLoadOptions](../../com.aspose.gridweb/gridloadoptions)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Hämtar det maximala visningskolumnindexet (nollbaserat) för webbläsarket. Kontrollens använder det större värdet av MaxColumn och bladdata's maxkolumn.

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


Hämtar det maximala visningsradindexet (nollbaserat) för webbläsarket. Kontrollens använder det större värdet av MaxRow och bladdata's maxrad.

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


Hämtar meddelandet för rutnätet.

**Returns:**
java.lang.String
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


Hämtar det minsta visningskolumnindexet (nollbaserat) för webbläsarket. Kontrollens använder det mindre värdet av MinColumn och bladdata's minkolumn.

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


Hämtar det minsta visningsradindexet (nollbaserat) för webbläsarket. Kontrollens använder det mindre värdet av MinRow och bladdata's minrad.

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


Hämtar samlingen av celler som har modifierats av klienten.

**Returns:**
java.util.ArrayList
### getNeedRenderGroupRows() {#getNeedRenderGroupRows--}
```
public boolean getNeedRenderGroupRows()
```


Hämtar om grouprows ska visas.

**Returns:**
boolean
### getNoHScroll() {#getNoHScroll--}
```
public boolean getNoHScroll()
```


Hämtar ett värde som indikerar om den horisontella rullningslisten är dold.

**Returns:**
boolean
### getNoScroll() {#getNoScroll--}
```
public boolean getNoScroll()
```


Hämtar om rullningslisten ska visas.

**Returns:**
boolean
### getNoVScroll() {#getNoVScroll--}
```
public boolean getNoVScroll()
```


Hämtar ett värde som indikerar om den vertikala rullningslisten är dold.

**Returns:**
boolean
### getOnAjaxCallFinishedClientFunction() {#getOnAjaxCallFinishedClientFunction--}
```
public String getOnAjaxCallFinishedClientFunction()
```


Hämtar klient‑sidans funktionsnamn som ska anropas när ajaxcall är klar. Klientfunktionen bör deklareras så här:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnCellErrorClientFunction() {#getOnCellErrorClientFunction--}
```
public String getOnCellErrorClientFunction()
```


Hämtar klient‑sidans funktionsnamn som ska anropas när en cells validering misslyckas. Klientfunktionen bör deklareras så här:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnCellSelectedAjaxCallBackClientFunction() {#getOnCellSelectedAjaxCallBackClientFunction--}
```
public String getOnCellSelectedAjaxCallBackClientFunction()
```


Hämtar klientsidans funktion som ska anropas när en cell är markerad. Klientfunktionen bör deklareras så här:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnCellSelectedClientFunction() {#getOnCellSelectedClientFunction--}
```
public String getOnCellSelectedClientFunction()
```


Hämtar klientsidans funktion som ska anropas när en cell är markerad. Klientfunktionen bör deklareras så här:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnCellUnselectedClientFunction() {#getOnCellUnselectedClientFunction--}
```
public String getOnCellUnselectedClientFunction()
```


Hämtar klientsidans funktion som ska anropas när en cell avmarkeras. Klientfunktionen bör deklareras så här:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnCellUpdatedClientFunction() {#getOnCellUpdatedClientFunction--}
```
public String getOnCellUpdatedClientFunction()
```


Hämtar namnet på klientsidans funktion som ska anropas när en cells värde uppdateras. Klientfunktionen bör deklareras så här:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnContextMenuShowClientFunction() {#getOnContextMenuShowClientFunction--}
```
public String getOnContextMenuShowClientFunction()
```


Hämtar klientsidans funktion som ska anropas när snabbmenyn ska visas. Klientfunktionen bör deklareras så här:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnDoubleClickCellClientFunction() {#getOnDoubleClickCellClientFunction--}
```
public String getOnDoubleClickCellClientFunction()
```


Hämtar klientsidans funktion som ska anropas när en cell dubbelklickas. Klientfunktionen bör deklareras så här:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnDoubleClickRowClientFunction() {#getOnDoubleClickRowClientFunction--}
```
public String getOnDoubleClickRowClientFunction()
```


Hämtar klientsidans funktion som ska anropas när en rad dubbelklickas. Klientfunktionen bör deklareras så här:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnGridInitClientFunction() {#getOnGridInitClientFunction--}
```
public String getOnGridInitClientFunction()
```


Hämtar namnet på klientsidans funktion som ska anropas när rutnätet initieras. Klientfunktionen bör deklareras så här:
function MyOnGridInit(grid)
\{
alert("Rutnätet är initierat: " + grid.id);
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnPageChangeClientFunction() {#getOnPageChangeClientFunction--}
```
public String getOnPageChangeClientFunction()
```


Hämtar klientsidans funktion som ska anropas efter sidindexändring. Gäller endast när EnablePaging är true. Klientfunktionen bör deklareras så här:
function MyOnPageChange(index)
\{
console.log("aktuell sida är:"+index);
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnPageSubmitClientFunction() {#getOnPageSubmitClientFunction--}
```
public String getOnPageSubmitClientFunction()
```


Hämtar klientfunktionen som ska anropas innan sidan skickas in på klientsidan.

**Returns:**
java.lang.String
### getOnShapeSelectedClientFunction() {#getOnShapeSelectedClientFunction--}
```
public String getOnShapeSelectedClientFunction()
```


Hämtar klient‑sidans funktion som ska anropas när en form väljs. Klientfunktionen bör deklareras så här:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnSubmitClientFunction() {#getOnSubmitClientFunction--}
```
public String getOnSubmitClientFunction()
```


Hämtar klientfunktionen som ska anropas innan kontrollen skickas från klienten. Klientfunktionen bör deklareras så här:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
Argumentet arg är inlämningsargumentet och innehåller kommandot som ska skickas till servern. cancelEdit är ett booleskt värde som indikerar om kontrollen har förkastat användarens inmatning innan inlämning. Kontrollens inlämning fortsätter om funktionen returnerar true.
Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Returns:**
java.lang.String
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Hämtar om endast rader vars höjd inte är anpassad ska passa, standardvärdet är false.

**Returns:**
boolean
### getPageSize() {#getPageSize--}
```
public int getPageSize()
```


Hämtar sidstorleken i pagineringsläge.

**Remarks**

När den är i sidindelningsläge visar kontrollen PageSize rader data en gång, och visar sidvalskontrollen i flikfältet.

**Returns:**
int
### getPictureCachePath() {#getPictureCachePath--}
```
public static String getPictureCachePath()
```


Hämtar bildlagringssökvägen för arbetsboken, alla former och bilder lagras i denna katalog, standardsökvägen är acwcache under den aktuella applikationens baskatalog. Användare måste implementera en schemalagd tjänst för att rensa filer som har gått utanför sessionstiden.

**Returns:**
java.lang.String
### getPresetStyle() {#getPresetStyle--}
```
public int getPresetStyle()
```


Hämtar den förinställda stilen.

Se [PresetStyle](../../com.aspose.gridweb/presetstyle).

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


Hämtar om valideringsvärdet ska uppdateras efter att cellvärdet ändras.

**Returns:**
boolean
### getRenderHiddenRow() {#getRenderHiddenRow--}
```
public boolean getRenderHiddenRow()
```


Hämtar om den dolda raden renderas i GridControl, standardvärdet är false. Om du senare behöver visa den dolda raden ska du sätta den till true.

**Returns:**
boolean
### getRowHeightForCSV() {#getRowHeightForCSV--}
```
public double getRowHeightForCSV()
```


Hämtar radens höjdvärde i punkter för csv‑fil, standardvärdet är 14,5.

**Returns:**
double
### getScrollBarArrowColor() {#getScrollBarArrowColor--}
```
public Color getScrollBarArrowColor()
```


Anger färgen på rullningslistens pilknapp.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getScrollBarBaseColor() {#getScrollBarBaseColor--}
```
public Color getScrollBarBaseColor()
```


Anger färgen på kontrollens rullningslist.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellBgColor() {#getSelectCellBgColor--}
```
public Color getSelectCellBgColor()
```


Anger bakgrundsfärgen för de markerade cellerna i ett flervalsområde.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCellColor() {#getSelectCellColor--}
```
public Color getSelectCellColor()
```


Anger färgen på de markerade cellerna i ett flervalsområde.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getSelectCells() {#getSelectCells--}
```
public ArrayList getSelectCells()
```


Hämtar samlingen av markerade celler.

**Returns:**
java.util.ArrayList
### getSessionStorePath() {#getSessionStorePath--}
```
public String getSessionStorePath()
```


Hämtar sökvägen för sessionscachelagring när sessionsläget är File eller ViewState, etc: gridweb.SessionStorePath="c:/mytempdir/session"; då lagras sessionsdata i c:/mytempdir/session

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public GridWorkbookSettings getSettings()
```


Representerar arbetsbokens inställningar.

**Returns:**
[GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings)
### getShowAddButton() {#getShowAddButton--}
```
public boolean getShowAddButton()
```


Hämtar om knappen för att lägga till kalkylblad ska visas.

**Returns:**
boolean
### getShowBottomBar() {#getShowBottomBar--}
```
public boolean getShowBottomBar()
```


Anger om kommandoraden (inkluderar kommandorad och flikrad) ska visas längst ner i kontrollen.

**Returns:**
boolean
### getShowCellEditBox() {#getShowCellEditBox--}
```
public boolean getShowCellEditBox()
```


Om Gridweb visar verktygsfält för redigeringsruta som i MS‑EXCEL. Om det är aktiverat visas en redigeringsruta för den aktuella cellen i Gridweb. Om vi aktiverar denna funktion måste du importera jquery‑js‑biblioteket i dina aspx‑filer för att stödja den nya funktionen. Alla senaste jquery‑versioner fungerar, osv.

**Returns:**
boolean
### getShowCommandBarAtTop() {#getShowCommandBarAtTop--}
```
public boolean getShowCommandBarAtTop()
```


Anger om kommandoraden (inkluderar kommandorad och flikrad) ska visas högst upp i kontrollen.

**Returns:**
boolean
### getShowContextMenu() {#getShowContextMenu--}
```
public boolean getShowContextMenu()
```


Hämtar om snabbmenyn ska visas. Standardvärdet är true.

**Returns:**
boolean
### getShowDefaultGridLine() {#getShowDefaultGridLine--}
```
public boolean getShowDefaultGridLine()
```


Hämtar om standardrutnätslinjerna för cellerna ska visas.

**Returns:**
boolean
### getShowHeaderBar() {#getShowHeaderBar--}
```
public boolean getShowHeaderBar()
```


Hämtar om rubrikfältet ska visas

**Returns:**
boolean
### getShowLoading() {#getShowLoading--}
```
public boolean getShowLoading()
```


Anger om en laddningsdialogruta ska visas under postback till servern.

**Returns:**
boolean
### getShowLoadingPosition() {#getShowLoadingPosition--}
```
public String getShowLoadingPosition()
```


Anger vänster- och topposition (i px) för att visa laddningsdialogrutan under postback till servern, osv. 100,200 betyder att laddningsdialogrutans vänster- och topposition är 100 px, 200 px.

**Returns:**
java.lang.String
### getShowSaveButton() {#getShowSaveButton--}
```
public boolean getShowSaveButton()
```


Hämtar om spara‑knappen ska visas.

**Returns:**
boolean
### getShowSubmitButton() {#getShowSubmitButton--}
```
public boolean getShowSubmitButton()
```


Hämtar om skicka‑knappen ska visas.

**Returns:**
boolean
### getShowTabBar() {#getShowTabBar--}
```
public boolean getShowTabBar()
```


Hämtar om flikfältet ska visas.

**Returns:**
boolean
### getShowTabNavigation() {#getShowTabNavigation--}
```
public boolean getShowTabNavigation()
```


Hämtar om fliknavigationsknappen visas, standardvärdet är true.

**Returns:**
boolean
### getShowUndoButton() {#getShowUndoButton--}
```
public boolean getShowUndoButton()
```


Hämtar om ångra‑knappen ska visas.

**Returns:**
boolean
### getSpanWrap() {#getSpanWrap--}
```
public boolean getSpanWrap()
```


Anger om innehållet ska radbrytas i cellspannet, standardvärdet är true.

**Returns:**
boolean
### getTabIndex() {#getTabIndex--}
```
public short getTabIndex()
```


Hämtar TabIndex i WebControl

**Returns:**
short
### getTabStyle() {#getTabStyle--}
```
public GridTableItemStyle getTabStyle()
```


Hämtar stilen för flikfältet.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle)
### getToolTip() {#getToolTip--}
```
public String getToolTip()
```


Hämtar ToolTip i WebControl

**Returns:**
java.lang.String
### getUseClientPageHeight() {#getUseClientPageHeight--}
```
public boolean getUseClientPageHeight()
```


Hämtar om GridWeb använder klientens sidhöjd som kontrollhöjd, lämpligt när Height="100%" är satt, standardvärdet är false.

**Returns:**
boolean
### getVersion() {#getVersion--}
```
public static String getVersion()
```


Hämta utgivningsversionen.

**Returns:**
java.lang.String - Versionsnumret.
### getViewPanelScrollLeft() {#getViewPanelScrollLeft--}
```
public String getViewPanelScrollLeft()
```


Hämtar positionen för rullningslisten i gridens visningspanel.

**Returns:**
java.lang.String
### getViewPanelScrollTop() {#getViewPanelScrollTop--}
```
public String getViewPanelScrollTop()
```


Hämtar positionen för rullningslisten i gridens visningspanel.

**Returns:**
java.lang.String
### getViewTableStyle() {#getViewTableStyle--}
```
public GridTableStyle getViewTableStyle()
```


Hämtar stilen för datavisningspanelen.

**Returns:**
[GridTableStyle](../../com.aspose.gridweb/gridtablestyle)
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Hämtar bredden (System.Web.UI.WebControl.Unit) för kontrollen.

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


Hämtar samlingen av arbetsblad.

**Returns:**
[GridWorksheetCollection](../../com.aspose.gridweb/gridworksheetcollection)
### getXhtmlMode() {#getXhtmlMode--}
```
public boolean getXhtmlMode()
```


Hämtar om XHTML‑stil ska användas, standardvärdet är true.

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


Importerar från en Excel‑filström, inklusive filström från disk eller minnesström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Excel‑filens ström, inklusive filström från disk eller minnesström. |

### importExcelFile(InputStream stream, String passwordtoOpen) {#importExcelFile-java.io.InputStream-java.lang.String-}
```
public void importExcelFile(InputStream stream, String passwordtoOpen)
```


Importerar från en Excel‑filström, inklusive filström från disk eller minnesström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Excel‑filens ström, inklusive filström från disk eller minnesström. |
| passwordtoOpen | java.lang.String | öppningslösenordet för den krypterade filen. |

### importExcelFile(String fileName) {#importExcelFile-java.lang.String-}
```
public void importExcelFile(String fileName)
```


Importerar från en Excel‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Excel‑filens namn. |

### importExcelFile(String fileName, String passwordtoOpen) {#importExcelFile-java.lang.String-java.lang.String-}
```
public void importExcelFile(String fileName, String passwordtoOpen)
```


Importerar från en Excel‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Excel‑filens namn. |
| passwordtoOpen | java.lang.String | öppningslösenordet för den krypterade filen. |

### isCalculateFormula() {#isCalculateFormula--}
```
public boolean isCalculateFormula()
```


Hämtar om formeln ska beräknas efter att cellvärdet ändras eller efter import av fil. Standardvärdet är true.

**Returns:**
boolean
### loadCSVFile(InputStream stream) {#loadCSVFile-java.io.InputStream-}
```
public void loadCSVFile(InputStream stream)
```


Läser in data från en CSV‑filström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Filströmmen. |

### loadCSVFile(String fileName) {#loadCSVFile-java.lang.String-}
```
public void loadCSVFile(String fileName)
```


Läser in data från en CSV‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filens namn. |

### loadHTMLFile(InputStream stream) {#loadHTMLFile-java.io.InputStream-}
```
public void loadHTMLFile(InputStream stream)
```


Läser in data från en HTML‑filström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Filströmmen. |

### loadHTMLFile(String fileName) {#loadHTMLFile-java.lang.String-}
```
public void loadHTMLFile(String fileName)
```


Läser in data från en HTML‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filens namn. |

### loadSpreadSheetMLFile(InputStream stream) {#loadSpreadSheetMLFile-java.io.InputStream-}
```
public void loadSpreadSheetMLFile(InputStream stream)
```


Läser in data från en SpreadSheetML‑filström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Filens ström. |

### loadSpreadSheetMLFile(String fileName) {#loadSpreadSheetMLFile-java.lang.String-}
```
public void loadSpreadSheetMLFile(String fileName)
```


Läser in data från en SpreadSheetML‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filens namn. |

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


uppdatera alla diagrambilder för det aktiva kalkylbladet.

### saveCSVFile(OutputStream stream) {#saveCSVFile-java.io.OutputStream-}
```
public void saveCSVFile(OutputStream stream)
```


Sparar data till en CSV-filström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Filströmmen. |

### saveCSVFile(String targetFile) {#saveCSVFile-java.lang.String-}
```
public void saveCSVFile(String targetFile)
```


Sparar data till en CSV-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| targetFile | java.lang.String | Filens namn. |

### saveCustomStyleFile(String fileName) {#saveCustomStyleFile-java.lang.String-}
```
public void saveCustomStyleFile(String fileName)
```


Sparar kontrollens aktuella stildata till en XML‑fil. Kan användas för att skapa din anpassade stilfil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Stilfilens namn. |

### saveHTMLFile(OutputStream stream) {#saveHTMLFile-java.io.OutputStream-}
```
public void saveHTMLFile(OutputStream stream)
```


Sparar data till en HTML-filström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Filströmmen. |

### saveHTMLFile(String targetFile) {#saveHTMLFile-java.lang.String-}
```
public void saveHTMLFile(String targetFile)
```


Sparar data till en HTML-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| targetFile | java.lang.String | Filens namn. |

### saveSpreadSheetMLFile(OutputStream stream) {#saveSpreadSheetMLFile-java.io.OutputStream-}
```
public void saveSpreadSheetMLFile(OutputStream stream)
```


Sparar data till en SpreadSheetML-filström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Filströmmen. |

### saveSpreadSheetMLFile(String targetFile) {#saveSpreadSheetMLFile-java.lang.String-}
```
public void saveSpreadSheetMLFile(String targetFile)
```


Sparar data till en SpreadSheetML-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| targetFile | java.lang.String | Filens namn. |

### saveToExcelFile(OutputStream stream) {#saveToExcelFile-java.io.OutputStream-}
```
public void saveToExcelFile(OutputStream stream)
```


Sparar arbetsbladen till en Excel-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen att skriva till. |

### saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions) {#saveToExcelFile-java.io.OutputStream-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(OutputStream stream, GridSaveOptions saveOptions)
```


Sparar arbetsbladen till en Excel-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen att skriva till. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Sparaalternativen. |

### saveToExcelFile(OutputStream stream, int format) {#saveToExcelFile-java.io.OutputStream-int-}
```
public void saveToExcelFile(OutputStream stream, int format)
```


Sparar arbetsbladen till en Excel-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.OutputStream | Strömmen att skriva till. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Filformatet (Excel2003, Excel2007, CSV, SpreadsheetML) |

### saveToExcelFile(String targetFile) {#saveToExcelFile-java.lang.String-}
```
public void saveToExcelFile(String targetFile)
```


Sparar arbetsbladen till en Excel-fil i Excel 2003-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| targetFile | java.lang.String | Namnet på målfilen att skriva till. |

### saveToExcelFile(String targetFile, GridSaveOptions saveOptions) {#saveToExcelFile-java.lang.String-com.aspose.gridweb.GridSaveOptions-}
```
public void saveToExcelFile(String targetFile, GridSaveOptions saveOptions)
```


Sparar arbetsbladen till en Excel-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| targetFile | java.lang.String | Namnet på målfilen att skriva till. |
| saveOptions | [GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions) | Sparaalternativen. |

### saveToExcelFile(String targetFile, int format) {#saveToExcelFile-java.lang.String-int-}
```
public void saveToExcelFile(String targetFile, int format)
```


Sparar arbetsbladen till en Excel-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| targetFile | java.lang.String | Namnet på målfilen att skriva till. |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Filformatet (Excel2003, Excel2007, CSV, SpreadsheetML) |

### setACWClientPath(String value) {#setACWClientPath-java.lang.String-}
```
public void setACWClientPath(String value)
```


Ställer in webbadressen för skript-/bildfilerna i kontrollen. Till exempel: "http://localhost/acw\_client". Du kan också ange detta värde i web.config-filen. Lägg till detta avsnitt i `<configuration>`-avsnittet:
`<appSettings>`
`<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />`
`</appSettings>`


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setACWLanguageFileUrl(String value) {#setACWLanguageFileUrl-java.lang.String-}
```
public void setACWLanguageFileUrl(String value)
```


Ställer in webbadressen för språkfilen i kontrollen. Till exempel: "/acw\_client/lang\_en.js".
Som standard används en inbyggd engelsk fil.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setActiveCell(GridCell value) {#setActiveCell-com.aspose.gridweb.GridCell-}
```
public void setActiveCell(GridCell value)
```


Ställer in den aktiva cellen i det aktuella bladet. Ändrad till skrivbar sedan version 1.9.0.1.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setActiveCellBgColor(Color value) {#setActiveCellBgColor-com.aspose.gridweb.Color-}
```
public void setActiveCellBgColor(Color value)
```


Anger bakgrundsfärgen för den aktiva cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveCellColor(Color value) {#setActiveCellColor-com.aspose.gridweb.Color-}
```
public void setActiveCellColor(Color value)
```


Anger färgen för den aktiva cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderBgColor(Color value) {#setActiveHeaderBgColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderBgColor(Color value)
```


Anger bakgrundsfärgen för den aktiva rad‑/kolumnrubriken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveHeaderColor(Color value) {#setActiveHeaderColor-com.aspose.gridweb.Color-}
```
public void setActiveHeaderColor(Color value)
```


Anger färgen för den aktiva rad‑/kolumnrubriken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Ställer in det aktiva bladets index. Motsvarar WebWorksheets.ActiveSheetIndex.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setActiveTabStyle(GridTableItemStyle value) {#setActiveTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setActiveTabStyle(GridTableItemStyle value)
```


Anger stilen för den aktiva fliken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setAutoRefreshChart(boolean value) {#setAutoRefreshChart-boolean-}
```
public void setAutoRefreshChart(boolean value)
```


Ställer in om diagrambilden uppdateras när cellvärdet uppdateras. standardvärdet är true

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


Ställer in BackColor i WebControl

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Ställer in BorderColor i WebControl

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Ställer in BorderStyle i WebControl

Se [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Ställer in BorderWidth i WebControl

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomTableStyle(GridTableStyle value) {#setBottomTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setBottomTableStyle(GridTableStyle value)
```


Ställer in stilen för kontrollens nedre verktygsfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Ställer in om formeln ska beräknas efter att cellvärdet ändras eller efter import av fil. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Ställer in CssClass i WebControl

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCurrentPageIndex(int value) {#setCurrentPageIndex-int-}
```
public void setCurrentPageIndex(int value)
```


Ställer in index för aktuell sida i pagineringsläge.

**Remarks**

När den är i sidindelningsläge visar kontrollen PageSize rader data en gång, och visar sidvalskontrollen i flikfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCustomCalculationEngine(GridAbstractCalculationEngine value) {#setCustomCalculationEngine-com.aspose.gridweb.GridAbstractCalculationEngine-}
```
public void setCustomCalculationEngine(GridAbstractCalculationEngine value)
```


Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridAbstractCalculationEngine](../../com.aspose.gridweb/gridabstractcalculationengine) |  |

### setCustomStyle(InputStream stream) {#setCustomStyle-java.io.InputStream-}
```
public void setCustomStyle(InputStream stream)
```


ställer in den anpassade stilfilen från en ström, inklusive filströmmar från disk eller minne.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stream | java.io.InputStream | Filens ström, inklusive diskfilström eller minnesström. |

### setCustomStyleFileName(String value) {#setCustomStyleFileName-java.lang.String-}
```
public void setCustomStyleFileName(String value)
```


Ställer in namn på den anpassade stilfilen.

**Remarks**

Den anpassade stilfilen är en XML-fil. När du anger filnamnet laddas filen omedelbart. Här är innehållet i den "standard förinställda stilen" ------------------------------------------------------- <Aspose.Cells.GridWeb.ViewerStyleTemplate runat="server" HeaderBarWidth="30pt" ScrollBarBaseColor="" FrameTableStyle-BorderStyle="Solid" FrameTableStyle-LeftBorderStyle-BorderWidth="" FrameTableStyle-LeftBorderStyle-BorderColor="" FrameTableStyle-RightBorderStyle-BorderWidth="" FrameTableStyle-RightBorderStyle-BorderColor="" FrameTableStyle-BorderWidth="1px" FrameTableStyle-CellSpacing="0" FrameTableStyle-BorderColor="Gray" FrameTableStyle-CellPadding="0" FrameTableStyle-TopBorderStyle-BorderWidth="" FrameTableStyle-TopBorderStyle-BorderColor="" FrameTableStyle-BottomBorderStyle-BorderWidth="" FrameTableStyle-BottomBorderStyle-BorderColor="" HeaderBarStyle-LeftBorderStyle-BorderStyle="Solid" HeaderBarStyle-LeftBorderStyle-BorderWidth="1px" HeaderBarStyle-LeftBorderStyle-BorderColor="White" HeaderBarStyle-VerticalAlign="Middle" HeaderBarStyle-RightBorderStyle-BorderStyle="Solid" HeaderBarStyle-RightBorderStyle-BorderWidth="1px" HeaderBarStyle-RightBorderStyle-BorderColor="Gray" HeaderBarStyle-BorderWidth="1px" HeaderBarStyle-Font-Size="10pt" HeaderBarStyle-BorderColor="Gray" HeaderBarStyle-BorderStyle="Solid" HeaderBarStyle-HorizontalAlign="Center" HeaderBarStyle-ForeColor="Black" HeaderBarStyle-TopBorderStyle-BorderStyle="Solid" HeaderBarStyle-TopBorderStyle-BorderWidth="1px" HeaderBarStyle-TopBorderStyle-BorderColor="White" HeaderBarStyle-BackColor="\#E0E0E0" HeaderBarStyle-BottomBorderStyle-BorderStyle="Solid" HeaderBarStyle-BottomBorderStyle-BorderWidth="1px" HeaderBarStyle-BottomBorderStyle-BorderColor="Gray" ViewTableStyle-LeftBorderStyle-BorderWidth="" ViewTableStyle-LeftBorderStyle-BorderColor="" ViewTableStyle-LayoutFixed="Fixed" ViewTableStyle-RightBorderStyle-BorderWidth="" ViewTableStyle-RightBorderStyle-BorderColor="" ViewTableStyle-BorderWidth="0px" ViewTableStyle-CellSpacing="0" ViewTableStyle-CellPadding="0" ViewTableStyle-TopBorderStyle-BorderWidth="" ViewTableStyle-TopBorderStyle-BorderColor="" ViewTableStyle-BottomBorderStyle-BorderWidth="" ViewTableStyle-BottomBorderStyle-BorderColor="" BottomTableStyle-LeftBorderStyle-BorderWidth="" BottomTableStyle-LeftBorderStyle-BorderColor="" BottomTableStyle-LayoutFixed="Fixed" BottomTableStyle-RightBorderStyle-BorderWidth="" BottomTableStyle-RightBorderStyle-BorderColor="" BottomTableStyle-BorderWidth="0px" BottomTableStyle-CellSpacing="0" BottomTableStyle-CellPadding="1" BottomTableStyle-TopBorderStyle-BorderStyle="Solid" BottomTableStyle-TopBorderStyle-BorderWidth="1px" BottomTableStyle-TopBorderStyle-BorderColor="Gray" BottomTableStyle-BottomBorderStyle-BorderWidth="" BottomTableStyle-BottomBorderStyle-BorderColor="" HeaderBarHeight="15pt" ActiveTabStyle-LeftBorderStyle-BorderWidth="" ActiveTabStyle-LeftBorderStyle-BorderColor="" ActiveTabStyle-RightBorderStyle-BorderWidth="" ActiveTabStyle-RightBorderStyle-BorderColor="" ActiveTabStyle-Height="15pt" ActiveTabStyle-BorderWidth="1px" ActiveTabStyle-Font-Size="10pt" ActiveTabStyle-BorderColor="Gray" ActiveTabStyle-ForeColor="Black" ActiveTabStyle-TopBorderStyle-BorderWidth="" ActiveTabStyle-TopBorderStyle-BorderColor="" ActiveTabStyle-BackColor="White" ActiveTabStyle-BottomBorderStyle-BorderWidth="" ActiveTabStyle-BottomBorderStyle-BorderColor="" HeaderBarTableStyle-LeftBorderStyle-BorderWidth="" HeaderBarTableStyle-LeftBorderStyle-BorderColor="" HeaderBarTableStyle-LayoutFixed="Fixed" HeaderBarTableStyle-RightBorderStyle-BorderWidth="" HeaderBarTableStyle-RightBorderStyle-BorderColor="" HeaderBarTableStyle-BorderWidth="0px" HeaderBarTableStyle-CellSpacing="0" HeaderBarTableStyle-BorderCollapse="Separate" HeaderBarTableStyle-CellPadding="0" HeaderBarTableStyle-TopBorderStyle-BorderWidth="" HeaderBarTableStyle-TopBorderStyle-BorderColor="" HeaderBarTableStyle-BottomBorderStyle-BorderWidth="" HeaderBarTableStyle-BottomBorderStyle-BorderColor="" TabStyle-LeftBorderStyle-BorderWidth="" TabStyle-LeftBorderStyle-BorderColor="" TabStyle-RightBorderStyle-BorderWidth="" TabStyle-RightBorderStyle-BorderColor="" TabStyle-Height="15pt" TabStyle-BorderWidth="1px" TabStyle-Font-Size="10pt" TabStyle-BorderColor="Gray" TabStyle-ForeColor="Black" TabStyle-TopBorderStyle-BorderWidth="" TabStyle-TopBorderStyle-BorderColor="" TabStyle-BackColor="\#E0E0E0" TabStyle-BottomBorderStyle-BorderWidth="" TabStyle-BottomBorderStyle-BorderColor="" ScrollBarArrowColor=""></Aspose.Cells.GridWeb.ViewerStyleTemplate>

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDPI(double value) {#setDPI-double-}
```
public static void setDPI(double value)
```


Hämtar /Ställer in DPI för maskinen.

**Remarks**

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Ställer in kontrollens standardteckensnittsnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


Ställer in kontrollens standardteckenstorlek.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setDefaultGridLineColor(Color value) {#setDefaultGridLineColor-com.aspose.gridweb.Color-}
```
public void setDefaultGridLineColor(Color value)
```


Ställer in standardfärgen för rutnätslinjer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setDisplayCellTip(boolean value) {#setDisplayCellTip-boolean-}
```
public void setDisplayCellTip(boolean value)
```


Ställer in om tips ska visas. standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEditMode(boolean value) {#setEditMode-boolean-}
```
public void setEditMode(boolean value)
```


Ställer in kontrollens redigeringsläge.

**Remarks**

När den är satt till true, är kontrollens celler redigerbara, och ikonerna "save" och "undo" visas. När den är satt till false, är kontrollens celler skrivskyddade, och ikonerna "save" och "undo" visas inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableAJAX(boolean value) {#setEnableAJAX-boolean-}
```
public void setEnableAJAX(boolean value)
```


Ställer in om AJAX-anrop ska användas. standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableAsync(boolean value) {#setEnableAsync-boolean-}
```
public void setEnableAsync(boolean value)
```


Ställer in om laddningsceller data ska hanteras asynkront, föreslås att tillämpas för ett blad med mer än 10000 celler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableClientColumnOperations(boolean value) {#setEnableClientColumnOperations-boolean-}
```
public void setEnableClientColumnOperations(boolean value)
```


Ställer in om kolumnoperationer på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren använda högerklicksmenyn för att lägga till/ta bort kolumner.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableClientFreeze(boolean value) {#setEnableClientFreeze-boolean-}
```
public void setEnableClientFreeze(boolean value)
```


Ställer in om frysningsoperationer på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren använda högerklicksmenyn för att frysa/töja paneler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableClientMergeOperations(boolean value) {#setEnableClientMergeOperations-boolean-}
```
public void setEnableClientMergeOperations(boolean value)
```


Ställer in om sammanslagningsoperationer på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren använda högerklicksmenyn för att slå ihop/ta isär celler.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableClientResizeColumnRow(boolean value) {#setEnableClientResizeColumnRow-boolean-}
```
public void setEnableClientResizeColumnRow(boolean value)
```


Ställer in om ändring av kolumn- och radstorlek på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren ändra storlek på kolumnen och raden på klientsidan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableClientRowOperations(boolean value) {#setEnableClientRowOperations-boolean-}
```
public void setEnableClientRowOperations(boolean value)
```


Ställer in om radoperationer på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren använda högerklicksmenyn för att lägga till/ta bort rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableDoubleClickEvent(boolean value) {#setEnableDoubleClickEvent-boolean-}
```
public void setEnableDoubleClickEvent(boolean value)
```


Ställer in om dubbelklickshändelse på kundsidan ska aktiveras.

**Remarks**

När den är satt till true kommer kontrollen att ta emot dubbelklickshändelser på kundsidan och du kan hantera dessa händelser på serversidan. Annars kommer kontrollen att ignorera alla dubbelklickshändelser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableMetalLightEffect(boolean value) {#setEnableMetalLightEffect-boolean-}
```
public void setEnableMetalLightEffect(boolean value)
```


Ställer in om metallljuseffekt ska tillämpas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnablePaging(boolean value) {#setEnablePaging-boolean-}
```
public void setEnablePaging(boolean value)
```


Ställer in om kontrollens sidindelningsläge ska aktiveras.

**Remarks**

När den är satt till true kommer kontrollen att visa PageSize rader med data på en gång, och visa sidvalskontrollen i flikfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableStyleDialogbox(boolean value) {#setEnableStyleDialogbox-boolean-}
```
public void setEnableStyleDialogbox(boolean value)
```


Ställer in om stil‑dialogrutan på klientsidan ska aktiveras.

**Remarks**

När den är satt till true kan användaren använda stil-dialogrutan för att sätta en cells stil genom att välja "Format Cell..." i popup-menyn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public void setEnabled(boolean value)
```


Ställer in Enabled i WebControl

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFilteredPaging(boolean value) {#setFilteredPaging-boolean-}
```
public void setFilteredPaging(boolean value)
```


Ställer in om sidindelning ska aktiveras efter att data filtrerats, påverkar när EnablePaging är sant.

**Remarks**

När den är satt till true kommer kontrollen att paginera baserat på filtrerade data, standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFontFolder(String fontFolder, boolean recursive) {#setFontFolder-java.lang.String-boolean-}
```
public static void setFontFolder(String fontFolder, boolean recursive)
```


Ställer in teckensnittsmappen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolder | java.lang.String | Mappen som innehåller TrueType-teckensnitt. |
| rekursiv | boolean | Bestämmer om underkataloger ska genomsökas eller inte. |

### setFontFolders(String[] fontFolders, boolean recursive) {#setFontFolders-java.lang.String---boolean-}
```
public static void setFontFolders(String[] fontFolders, boolean recursive)
```


Ställer in teckensnittsmapparna

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontFolders | java.lang.String[] | Mapparna som innehåller TrueType-teckensnitt. |
| rekursiv | boolean | Bestämmer om underkataloger ska genomsökas eller inte. |

### setForceValidation(boolean value) {#setForceValidation-boolean-}
```
public void setForceValidation(boolean value)
```


Ställer in om validering på kundsidan ska tvingas.

**Remarks**

När den är satt till true kommer data inte att skickas till servern förrän alla inmatningsfält är giltiga.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Ställer in ForeColor i WebControl

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setFrameTableStyle(GridTableStyle value) {#setFrameTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setFrameTableStyle(GridTableStyle value)
```


Ställer in ramstilen för kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setGoonDefaultSaveOperation(boolean value) {#setGoonDefaultSaveOperation-boolean-}
```
public void setGoonDefaultSaveOperation(boolean value)
```


Ställer in om GridWeb ska utföra standard‑sparoperation, standardvärdet är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHeaderBarHeight(Unit value) {#setHeaderBarHeight-com.aspose.gridweb.Unit-}
```
public void setHeaderBarHeight(Unit value)
```


Ställer in höjden (System.Web.UI.WebControl.Unit) för kontrollens övre rubrikrad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeaderBarStyle(GridTableItemStyle value) {#setHeaderBarStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setHeaderBarStyle(GridTableItemStyle value)
```


Ställer in rubrikradens stil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setHeaderBarTableStyle(GridTableStyle value) {#setHeaderBarTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setHeaderBarTableStyle(GridTableStyle value)
```


Ställer in rubrikradens stil för kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setHeaderBarWidth(Unit value) {#setHeaderBarWidth-com.aspose.gridweb.Unit-}
```
public void setHeaderBarWidth(Unit value)
```


Ställer in bredden (System.Web.UI.WebControl.Unit) för kontrollens vänstra rubrikrad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Ställer in höjden (System.Web.UI.WebControl.Unit) för kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setIgnoreStyleWithNoData(boolean value) {#setIgnoreStyleWithNoData-boolean-}
```
public void setIgnoreStyleWithNoData(boolean value)
```


Ställer in om GridWeb ignorerar att visa rader eller kolumner som inte innehåller cellvärden men ändå är stylade. Om den sätts till true blir prestandan bättre. Standardvärdet är false, vilket betyder att om den sista på varandra följande raden/kolumnen saknar cellvärden men är stylad, kommer vi fortfarande att visa dem. Detta alternativ är endast giltigt när EnableAsync är false. Detta alternativ har ingen effekt när EnableAsync är true, vilket betyder att GridWeb kommer att visa alla rader/kolumner med stil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLoadOptions(GridLoadOptions value) {#setLoadOptions-com.aspose.gridweb.GridLoadOptions-}
```
public void setLoadOptions(GridLoadOptions value)
```


Representerar laddningsalternativen för GridWeb.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridLoadOptions](../../com.aspose.gridweb/gridloadoptions) |  |

### setMaxColumn(int value) {#setMaxColumn-int-}
```
public void setMaxColumn(int value)
```


Ställer in det maximala visningskolumnindexet (nollbaserat) för webblådet. Kontrollens använder det större värdet av MaxColumn och bladdata's max column.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMaxRow(int value) {#setMaxRow-int-}
```
public void setMaxRow(int value)
```


Ställer in det maximala visningsradindexet (nollbaserat) för webblådet. Kontrollens använder det större värdet av MaxRow och bladdata's max row.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMessage(String value) {#setMessage-java.lang.String-}
```
public void setMessage(String value)
```


Ställer in meddelandet för rutnätet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setMinColumn(int value) {#setMinColumn-int-}
```
public void setMinColumn(int value)
```


Ställer in det minsta visningskolumnindexet (nollbaserat) för webblådet. Kontrollens använder det mindre värdet av MinColumn och bladdata's min column.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMinRow(int value) {#setMinRow-int-}
```
public void setMinRow(int value)
```


Ställer in det minsta visningsradindexet (nollbaserat) för webblådet. Kontrollens använder det mindre värdet av MinRow och bladdata's min row.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setNeedRenderGroupRows(boolean value) {#setNeedRenderGroupRows-boolean-}
```
public void setNeedRenderGroupRows(boolean value)
```


Ställer in om grupprader ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setNoHScroll(boolean value) {#setNoHScroll-boolean-}
```
public void setNoHScroll(boolean value)
```


Ställer in ett värde som indikerar om den horisontella rullningslisten är dold.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setNoScroll(boolean value) {#setNoScroll-boolean-}
```
public void setNoScroll(boolean value)
```


Ställer in om rullningslisten ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setNoVScroll(boolean value) {#setNoVScroll-boolean-}
```
public void setNoVScroll(boolean value)
```


Ställer in ett värde som indikerar om den vertikala rullningslisten är dold.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOnAjaxCallFinishedClientFunction(String value) {#setOnAjaxCallFinishedClientFunction-java.lang.String-}
```
public void setOnAjaxCallFinishedClientFunction(String value)
```


Ställer in klient-sidans funktionsnamn som ska anropas när ajax-anropet är klart. Klientfunktionen bör deklareras så här:
function GridAjaxcallFinished()
\{
alert(this.id+" ajaxcall finished ");
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnCellErrorClientFunction(String value) {#setOnCellErrorClientFunction-java.lang.String-}
```
public void setOnCellErrorClientFunction(String value)
```


Ställer in klient-sidans funktionsnamn som ska anropas när en cells validering misslyckas. Klientfunktionen bör deklareras så här:
function MyOnCellError(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnCellSelectedAjaxCallBackClientFunction(String value) {#setOnCellSelectedAjaxCallBackClientFunction-java.lang.String-}
```
public void setOnCellSelectedAjaxCallBackClientFunction(String value)
```


Ställer in klient-sidans funktion som ska anropas när en cell väljs. Klientfunktionen bör deklareras så här:
function MyOnSelectCellAjaxCallBack(cell,customerdata)
\{

\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnCellSelectedClientFunction(String value) {#setOnCellSelectedClientFunction-java.lang.String-}
```
public void setOnCellSelectedClientFunction(String value)
```


Ställer in klient-sidans funktion som ska anropas när en cell väljs. Klientfunktionen bör deklareras så här:
function MyOnSelectCell(cell)
\{
GridWeb1.setCellValueByCell(cell, "test");
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnCellUnselectedClientFunction(String value) {#setOnCellUnselectedClientFunction-java.lang.String-}
```
public void setOnCellUnselectedClientFunction(String value)
```


Ställer in klient-sidans funktion som ska anropas när en cell avmarkeras. Klientfunktionen bör deklareras så här:
function MyOnUnselectCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnCellUpdatedClientFunction(String value) {#setOnCellUpdatedClientFunction-java.lang.String-}
```
public void setOnCellUpdatedClientFunction(String value)
```


Ställer in klient-sidans funktionsnamn som ska anropas när en cells värde uppdateras. Klientfunktionen bör deklareras så här:
function MyOnCellUpdated(cell)
\{
alert(this.getCellValueByCell(cell));
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnContextMenuShowClientFunction(String value) {#setOnContextMenuShowClientFunction-java.lang.String-}
```
public void setOnContextMenuShowClientFunction(String value)
```


Ställer in klient-sidans funktion som ska anropas när snabbmenyn visas. Klientfunktionen bör deklareras så här:
function onContextMenuShow()
\{
var menu = event.srcElement;
menu.setItemVisibility("Delete", "block");
menu.setItemVisibility("Update", "none");
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnDoubleClickCellClientFunction(String value) {#setOnDoubleClickCellClientFunction-java.lang.String-}
```
public void setOnDoubleClickCellClientFunction(String value)
```


Ställer in klient-sidans funktion som ska anropas när en cell dubbelklickas. Klientfunktionen bör deklareras så här:
function MyOnDoubleClickCell(cell)
\{
this.setCellValueByCell(cell, "test");
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnDoubleClickRowClientFunction(String value) {#setOnDoubleClickRowClientFunction-java.lang.String-}
```
public void setOnDoubleClickRowClientFunction(String value)
```


Ställer in klient-sidans funktion som ska anropas när en rad dubbelklickas. Klientfunktionen bör deklareras så här:
function MyOnRowDoubleClick(row)
\{
alert(row);
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnGridInitClientFunction(String value) {#setOnGridInitClientFunction-java.lang.String-}
```
public void setOnGridInitClientFunction(String value)
```


Ställer in klient-sidans funktionsnamn som ska anropas när rutnätet initieras. Klientfunktionen bör deklareras så här:
function MyOnGridInit(grid)
\{
alert("Rutnätet är initierat: " + grid.id);
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnPageChangeClientFunction(String value) {#setOnPageChangeClientFunction-java.lang.String-}
```
public void setOnPageChangeClientFunction(String value)
```


Ställer in klient-sidans funktion som ska anropas efter att sidindex har ändrats. Gäller endast när EnablePaging är true. Klientfunktionen bör deklareras så här:
function MyOnPageChange(index)
\{
console.log("aktuell sida är:"+index);
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnPageSubmitClientFunction(String value) {#setOnPageSubmitClientFunction-java.lang.String-}
```
public void setOnPageSubmitClientFunction(String value)
```


Ställer in klientfunktionen som ska anropas innan sidan skickas från klienten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnShapeSelectedClientFunction(String value) {#setOnShapeSelectedClientFunction-java.lang.String-}
```
public void setOnShapeSelectedClientFunction(String value)
```


Ställer in klient-sidans funktion som ska anropas när en form väljs. Klientfunktionen bör deklareras så här:
function MyOnSelectShape(shape)
\{
var name=shape.getAttribute("namevalue")
var text=shape.getAttribute("textvalue")
var value=shape.getAttribute("controlvalue")
var type=shape.getAttribute("msotype")
\}

Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnSubmitClientFunction(String value) {#setOnSubmitClientFunction-java.lang.String-}
```
public void setOnSubmitClientFunction(String value)
```


Ställer in klientfunktionen som ska anropas innan kontrollen skickas på klientsidan. Klientfunktionen bör deklareras så här:
function MyOnSubmit(arg, cancelEdit)
\{
return true;
\}
Argumentet arg är inlämningsargumentet och innehåller kommandot som ska skickas till servern. cancelEdit är ett booleskt värde som indikerar om kontrollen har förkastat användarens inmatning innan inlämning. Kontrollens inlämning fortsätter om funktionen returnerar true.
Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på grid‑kontrollen som avfyrar händelsen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


Ställer in om endast rader vars höjd inte är anpassad ska anpassas, standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPageSize(int value) {#setPageSize-int-}
```
public void setPageSize(int value)
```


Ställer in sidstorleken i pagineringsläge.

**Remarks**

När den är i sidindelningsläge visar kontrollen PageSize rader data en gång, och visar sidvalskontrollen i flikfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPictureCachePath(String value) {#setPictureCachePath-java.lang.String-}
```
public static void setPictureCachePath(String value)
```


Ställer in bildlagringssökvägen för arbetsboken, alla former och bilder lagras i den här katalogen, standardsökvägen är acwcache under den aktuella applikationens baskatalog. Användare måste implementera en schemalagd tjänst för att rensa filer som har gått utanför sessionstiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPresetStyle(int value) {#setPresetStyle-int-}
```
public void setPresetStyle(int value)
```


Ställer in den förinställda stilen.

Se [PresetStyle](../../com.aspose.gridweb/presetstyle).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRefreshValidation(boolean value) {#setRefreshValidation-boolean-}
```
public void setRefreshValidation(boolean value)
```


Ställer in om valideringsvärdet ska uppdateras efter att cellvärdet ändras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRenderHiddenRow(boolean value) {#setRenderHiddenRow-boolean-}
```
public void setRenderHiddenRow(boolean value)
```


Ställer in om den dolda raden renderas i GridControl, standardvärdet är false. Om du behöver visa den dolda raden senare, ska du sätta den till true

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRowHeightForCSV(double value) {#setRowHeightForCSV-double-}
```
public void setRowHeightForCSV(double value)
```


Ställer in radens höjd i punkter för CSV‑fil, standardvärdet är 14,5.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setScrollBarArrowColor(Color value) {#setScrollBarArrowColor-com.aspose.gridweb.Color-}
```
public void setScrollBarArrowColor(Color value)
```


Anger färgen på rullningslistens pilknapp.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setScrollBarBaseColor(Color value) {#setScrollBarBaseColor-com.aspose.gridweb.Color-}
```
public void setScrollBarBaseColor(Color value)
```


Anger färgen på kontrollens rullningslist.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellBgColor(Color value) {#setSelectCellBgColor-com.aspose.gridweb.Color-}
```
public void setSelectCellBgColor(Color value)
```


Anger bakgrundsfärgen för de markerade cellerna i ett flervalsområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSelectCellColor(Color value) {#setSelectCellColor-com.aspose.gridweb.Color-}
```
public void setSelectCellColor(Color value)
```


Anger färgen på de markerade cellerna i ett flervalsområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setSessionStorePath(String value) {#setSessionStorePath-java.lang.String-}
```
public void setSessionStorePath(String value)
```


Ställer in sökvägen för sessionscachelagring när sessionsläget är File eller ViewState, t.ex.: gridweb.SessionStorePath=\"c:/mytempdir/session\"; då lagras sessionsdata i c:/mytempdir/session.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setSettings(GridWorkbookSettings value) {#setSettings-com.aspose.gridweb.GridWorkbookSettings-}
```
public void setSettings(GridWorkbookSettings value)
```


Representerar arbetsbokens inställningar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridWorkbookSettings](../../com.aspose.gridweb/gridworkbooksettings) |  |

### setShowAddButton(boolean value) {#setShowAddButton-boolean-}
```
public void setShowAddButton(boolean value)
```


Ställer in om knappen för att lägga till kalkylblad ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowBottomBar(boolean value) {#setShowBottomBar-boolean-}
```
public void setShowBottomBar(boolean value)
```


Anger om kommandoraden (inkluderar kommandorad och flikrad) ska visas längst ner i kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowCellEditBox(boolean value) {#setShowCellEditBox-boolean-}
```
public void setShowCellEditBox(boolean value)
```


Om Gridweb visar verktygsfält för redigeringsruta som i MS‑EXCEL. Om det är aktiverat visas en redigeringsruta för den aktuella cellen i Gridweb. Om vi aktiverar denna funktion måste du importera jquery‑js‑biblioteket i dina aspx‑filer för att stödja den nya funktionen. Alla senaste jquery‑versioner fungerar, osv.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowCommandBarAtTop(boolean value) {#setShowCommandBarAtTop-boolean-}
```
public void setShowCommandBarAtTop(boolean value)
```


Anger om kommandoraden (inkluderar kommandorad och flikrad) ska visas högst upp i kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowContextMenu(boolean value) {#setShowContextMenu-boolean-}
```
public void setShowContextMenu(boolean value)
```


Ställer in om snabbmenyn ska visas. standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowDefaultGridLine(boolean value) {#setShowDefaultGridLine-boolean-}
```
public void setShowDefaultGridLine(boolean value)
```


Ställer in om cellernas standardrutlinjer ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowHeaderBar(boolean value) {#setShowHeaderBar-boolean-}
```
public void setShowHeaderBar(boolean value)
```


Ställer in om rubrikfältet ska visas

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowLoading(boolean value) {#setShowLoading-boolean-}
```
public void setShowLoading(boolean value)
```


Anger om en laddningsdialogruta ska visas under postback till servern.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowLoadingPosition(String value) {#setShowLoadingPosition-java.lang.String-}
```
public void setShowLoadingPosition(String value)
```


Anger vänster- och topposition (i px) för att visa laddningsdialogrutan under postback till servern, osv. 100,200 betyder att laddningsdialogrutans vänster- och topposition är 100 px, 200 px.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setShowSaveButton(boolean value) {#setShowSaveButton-boolean-}
```
public void setShowSaveButton(boolean value)
```


Ställer in om spara-knappen ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowSubmitButton(boolean value) {#setShowSubmitButton-boolean-}
```
public void setShowSubmitButton(boolean value)
```


Ställer in om skicka-knappen ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowTabBar(boolean value) {#setShowTabBar-boolean-}
```
public void setShowTabBar(boolean value)
```


Ställer in om flikfältet ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowTabNavigation(boolean value) {#setShowTabNavigation-boolean-}
```
public void setShowTabNavigation(boolean value)
```


Ställer in om fliknavigationsknappen ska visas, standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowUndoButton(boolean value) {#setShowUndoButton-boolean-}
```
public void setShowUndoButton(boolean value)
```


Ställer in om ångra-knappen ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSpanWrap(boolean value) {#setSpanWrap-boolean-}
```
public void setSpanWrap(boolean value)
```


Anger om innehållet ska radbrytas i cellspannet, standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTabIndex(short value) {#setTabIndex-short-}
```
public void setTabIndex(short value)
```


Ställer in TabIndex i WebControl

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | short |  |

### setTabStyle(GridTableItemStyle value) {#setTabStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setTabStyle(GridTableItemStyle value)
```


Ställer in stilen för flikfältet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setToolTip(String value) {#setToolTip-java.lang.String-}
```
public void setToolTip(String value)
```


Ställer in ToolTip i WebControl

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setUseClientPageHeight(boolean value) {#setUseClientPageHeight-boolean-}
```
public void setUseClientPageHeight(boolean value)
```


Ställer in om GridWeb ska använda klientens sidhöjd som kontrollhöjd, lämpligt när Height="100%" är satt, standardvärdet är false

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setViewPanelScrollLeft(String value) {#setViewPanelScrollLeft-java.lang.String-}
```
public void setViewPanelScrollLeft(String value)
```


Ställer in positionen för rullningslisten i rutnätets visningspanel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setViewPanelScrollTop(String value) {#setViewPanelScrollTop-java.lang.String-}
```
public void setViewPanelScrollTop(String value)
```


Ställer in positionen för rullningslisten i rutnätets visningspanel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setViewTableStyle(GridTableStyle value) {#setViewTableStyle-com.aspose.gridweb.GridTableStyle-}
```
public void setViewTableStyle(GridTableStyle value)
```


Ställer in stilen för datavisningspanelen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridTableStyle](../../com.aspose.gridweb/gridtablestyle) |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Ställer in bredden (System.Web.UI.WebControl.Unit) för kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setXhtmlMode(boolean value) {#setXhtmlMode-boolean-}
```
public void setXhtmlMode(boolean value)
```


Ställer in om XHTML-stil ska användas, standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

