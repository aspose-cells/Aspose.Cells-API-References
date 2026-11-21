---
title: "HtmlSaveOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att spara html-fil."
type: docs
url: /sv/java/com.aspose.cells/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class HtmlSaveOptions extends SaveOptions
```

Representerar alternativen för att spara html-fil.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Skapar alternativ för att spara en html-fil. |
| [HtmlSaveOptions(int saveFormat)](#HtmlSaveOptions-int-) | Skapar alternativ för att spara en htm-fil. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddGenericFont()](#getAddGenericFont--) | Anger om en generisk teckensnitt ska läggas till i CSS font-family. |
| [getAddTooltipText()](#getAddTooltipText--) | Anger om tooltip-text ska läggas till när data inte kan visas helt. |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Den katalog som de bifogade filerna kommer att sparas till. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | Ange URL-prefixet för bifogade filer såsom bild i html-filen. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Mappen för temporära filer som kan användas som datacache. |
| [getCalculateFormula()](#getCalculateFormula--) | Anger om formler ska beräknas innan html-filen sparas. |
| [getCellCssPrefix()](#getCellCssPrefix--) | Hämtar prefixet för css-namnet, standardvärdet är "". |
| [getCellNameAttribute()](#getCellNameAttribute--) | Specificerar attributet som anger CellName som ska skrivas. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Gör arbetsboken tom efter att filen har sparats. |
| [getCreateDirectory()](#getCreateDirectory--) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [getCssStyles()](#getCssStyles--) | Hämtar de extra css-stilarna för formateraren. |
| [getDataBarRenderMode()](#getDataBarRenderMode--) | Representerar läget för hur DataBar renderas när Excel-filer konverteras till html-filer. |
| [getDefaultFontName()](#getDefaultFontName--) | Ange standardteckensnittets namn för export av html, standardteckensnittet kommer att användas när stilens teckensnitt inte finns, om detta egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null. |
| [getDisableCss()](#getDisableCss--) | Anger om endast inline-stilar ska tillämpas, utan att förlita sig på CSS. |
| [getDisableDownlevelRevealedComments()](#getDisableDownlevelRevealedComments--) | Anger om Downlevel-revealed villkorliga kommentarer ska inaktiveras vid export av fil till html, standardvärdet är false. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Hämtar typen av inbäddning av teckensnittsfiler i html-filen. |
| [getEnableCssCustomProperties()](#getEnableCssCustomProperties--) | Optimera html-utdata genom att använda anpassade CSS-egenskaper. |
| [getEncodeEntityAsCode()](#getEncodeEntityAsCode--) | Anger om html-teckenentiteter ersätts med decimalkod. |
| [getEncoding()](#getEncoding--) | Om inte angivet, använd Encoding.UTF8 som standardkodningstyp. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [getExcludeUnusedStyles()](#getExcludeUnusedStyles--) | Anger om oanvända stilar ska uteslutas. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Anger om endast det aktiva kalkylbladet ska exporteras till html-filen. |
| [getExportArea()](#getExportArea--) | Hämtar den exporterade CellArea för det aktuella aktiva kalkylbladet. |
| [getExportBogusRowData()](#getExportBogusRowData--) | Anger om export av felaktiga data i den sista raden. |
| [getExportCellCoordinate()](#getExportCellCoordinate--) | Anger om Excel-koordinater för icke tomma celler exporteras när filen sparas som HTML. |
| [getExportCommentsType()](#getExportCommentsType--) | Representerar typ av export av kommentarer till HTML-filer. |
| [getExportDataOptions()](#getExportDataOptions--) | Anger regeln för export av HTML-fildata. Standardvärdet är Alla. |
| [getExportDocumentProperties()](#getExportDocumentProperties--) | Anger om dokumentegenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet. |
| [getExportExtraHeadings()](#getExportExtraHeadings--) | Anger om extra rubriker exporteras när textens längd överstiger maximal visningskolumn. |
| [getExportFormula()](#getExportFormula--) | Anger om formler exporteras när filen sparas som HTML. |
| [getExportFrameScriptsAndProperties()](#getExportFrameScriptsAndProperties--) | Anger om ramskript och dokumentegenskaper exporteras. |
| [getExportGridLines()](#getExportGridLines--) | Anger om rutnätslinjer exporteras. Standardvärdet är false. |
| [getExportHeadings()](#getExportHeadings--) | Anger om bladets rad- och kolumnrubriker exporteras när du sparar till HTML-filer. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Anger om dolt kalkylbladsinnehåll exporteras. Standardvärdet är true. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB. |
| [getExportNamedRangeAnchors()](#getExportNamedRangeAnchors--) | Anger om ankarelement för namngivna områden exporteras när du sparar som HTML. |
| [getExportObjectListener()](#getExportObjectListener--) | Hämtar ExportObjectListener för export av objekt. |
| [getExportPageFooters()](#getExportPageFooters--) | Anger om sidhuvuden exporteras. |
| [getExportPageHeaders()](#getExportPageHeaders--) | Anger om sidhuvuden exporteras. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Anger om endast utskriftsområdet exporteras till HTML-filen. |
| [getExportRowColumnHeadings()](#getExportRowColumnHeadings--) | Anger om bladets rad- och kolumnrubriker exporteras när du sparar till HTML-filer. |
| [getExportSimilarBorderStyle()](#getExportSimilarBorderStyle--) | Anger om liknande kantlinjestil exporteras när kantlinjestilen inte stöds av webbläsare. |
| [getExportSingleTab()](#getExportSingleTab--) | Anger om den enda fliken exporteras när filen bara har ett kalkylblad. |
| [getExportWorkbookProperties()](#getExportWorkbookProperties--) | Anger om arbetsboks egenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet. |
| [getExportWorksheetCSSSeparately()](#getExportWorksheetCSSSeparately--) | Anger om kalkylbladets CSS exporteras separat. Standardvärdet är false. |
| [getExportWorksheetProperties()](#getExportWorksheetProperties--) | Anger om kalkylblads egenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet. |
| [getFilePathProvider()](#getFilePathProvider--) | Hämtar IFilePathProvider för separat export av kalkylblad till HTML. |
| [getFormatDataIgnoreColumnWidth()](#getFormatDataIgnoreColumnWidth--) | Anger om hela formaterade celldata visas när den överskrider kolumnen. |
| [getHiddenColDisplayType()](#getHiddenColDisplayType--) | Dold kolumn (bredden på denna kolumn är 0) i Excel, innan du sparar detta i HTML-format, om HtmlHiddenColDisplayType är "Remove" kommer den dolda kolumnen inte att skrivas ut, om värdet är "Hidden" kommer kolumnen att skrivas ut men vara dold, standardvärdet är "Hidden". |
| [getHiddenRowDisplayType()](#getHiddenRowDisplayType--) | Dold rad (höjden på den här raden är 0) i excel, innan du sparar detta i html-format, om HtmlHiddenRowDisplayType är "Remove" så kommer den dolda raden inte att skrivas ut, om värdet är "Hidden" så kommer raden att skrivas ut men vara dold, standardvärdet är "Hidden". |
| [getHideOverflowWrappedText()](#getHideOverflowWrappedText--) | Anger om överskjutande text ska döljas när cellformatet är inställt på radbrytning. |
| [getHtmlCrossStringType()](#getHtmlCrossStringType--) | Anger om en sträng som sträcker sig över flera celler ska visas på samma sätt som i MS Excel när en Excel-fil sparas i html-format. |
| [getHtmlVersion()](#getHtmlVersion--) | Specificerar version av HTML-standarden som ska användas när HTML-formatet sparas. |
| [getIgnoreInvisibleShapes()](#getIgnoreInvisibleShapes--) | Anger om osynliga former ska exporteras. |
| [getImageOptions()](#getImageOptions--) | Hämta ImageOrPrintOptions-objektet innan export. |
| [getImageScalable()](#getImageScalable--) | Anger om skalbar enhet ska användas för att beskriva bildens bredd när skalbar enhet används för att beskriva kolumnens bredd. |
| [getLayoutMode()](#getLayoutMode--) | Hämtar layoutläget när du sparar till HTML. |
| [getLinkTargetType()](#getLinkTargetType--) | Anger typen av target-attribut i `<a>`-länk. |
| [getMergeAreas()](#getMergeAreas--) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [getMergeEmptyTdForcely()](#getMergeEmptyTdForcely--) | Anger om tomma TD-element ska slås ihop tvångsmässigt vid export av fil till html. |
| [getMergeEmptyTdType()](#getMergeEmptyTdType--) | Alternativet för att slå ihop intilliggande tomma celler (tomma td-element). Standardvärdet är MergeEmptyTdType.Default. |
| [getOfficeMathOutputMode()](#getOfficeMathOutputMode--) | Anger hur OfficeMath-objekt exporteras till HTML, standardvärdet är Image. |
| [getPageTitle()](#getPageTitle--) | Titeln på html-sidan. |
| [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Anger om html-taggar (såsom `<div></div>`) i cellen ska tolkas som cellvärde eller bevaras som de är. |
| [getPresentationPreference()](#getPresentationPreference--) | Anger om html- eller mht-fil är presentationspreferens. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Anger om den senaste diagramdata ska cachas. |
| [getSaveAsSingleFile()](#getSaveAsSingleFile--) | Anger om html ska sparas som en enda fil. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar filformatet för sparning. |
| [getSheetSet()](#getSheetSet--) | Hämtar bladen som ska renderas. |
| [getShowAllSheets()](#getShowAllSheets--) | Anger om alla blad ska visas när du sparar som en enda html-fil. |
| [getSortExternalNames()](#getSortExternalNames--) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [getSortNames()](#getSortNames--) | Anger om definierade namn ska sorteras innan filen sparas. |
| [getSpaceMode()](#getSpaceMode--) | Anger hur mellanslag renderas i HTML-utdata. |
| [getStreamProvider()](#getStreamProvider--) | Hämtar IStreamProvider för att exportera objekt. |
| [getTableCssId()](#getTableCssId--) | Hämtar prefixet för typens CSS-namn såsom tr, col, td osv., de finns i tabellelementet som har det specifika TableCssId-attributet. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Anger om inställning för SmartArt ska uppdateras. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [getWarningCallback()](#getWarningCallback--) | Hämtar varningsåteranrop. |
| [getWidthScalable()](#getWidthScalable--) | Anger om kolumnbredd ska exporteras i skalanhet till html. |
| [getWorksheetScalable()](#getWorksheetScalable--) | Anger om html ska zoomas in eller ut via arbetsbladets zoomnivå när filen sparas till html, standardvärdet är false. |
| [hashCode()](#hashCode--) |  |
| [isBorderCollapsed()](#isBorderCollapsed--) | Anger om tabellramarna är sammanslagna. |
| [isExpImageToTempDir()](#isExpImageToTempDir--) | Anger om bildfiler ska exporteras till en temporär katalog. |
| [isExportComments()](#isExportComments--) | Anger om kommentarer exporteras när filen sparas till html, standardvärdet är falskt. |
| [isFullPathLink()](#isFullPathLink--) | Anger om fullständig sökvägslänk används i sheet00x.htm, filelist.xml och tabstrip.htm. |
| [isIECompatible()](#isIECompatible--) | Anger om den genererade HTML är kompatibel med IE‑webbläsaren. |
| [isJsBrowserCompatible()](#isJsBrowserCompatible--) | Anger om JavaScript är kompatibel med webbläsare som inte stödjer JavaScript. |
| [isMobileCompatible()](#isMobileCompatible--) | Anger om den genererade HTML är kompatibel med mobila enheter. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddGenericFont(boolean value)](#setAddGenericFont-boolean-) | Anger om en generisk teckensnitt ska läggas till i CSS font-family. |
| [setAddTooltipText(boolean value)](#setAddTooltipText-boolean-) | Anger om tooltip-text ska läggas till när data inte kan visas helt. |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Den katalog som de bifogade filerna kommer att sparas till. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | Ange URL-prefixet för bifogade filer såsom bild i html-filen. |
| [setBorderCollapsed(boolean value)](#setBorderCollapsed-boolean-) | Anger om tabellramarna är sammanslagna. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Mappen för temporära filer som kan användas som datacache. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Anger om formler ska beräknas innan html-filen sparas. |
| [setCellCssPrefix(String value)](#setCellCssPrefix-java.lang.String-) | Ställer in prefixet för css‑namnet, standardvärdet är "". |
| [setCellNameAttribute(String value)](#setCellNameAttribute-java.lang.String-) | Specificerar attributet som anger CellName som ska skrivas. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setClearData(boolean value)](#setClearData-boolean-) | Gör arbetsboken tom efter att filen har sparats. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [setCssStyles(String value)](#setCssStyles-java.lang.String-) | Ställer in ytterligare css‑stilar för formateraren. |
| [setDataBarRenderMode(int value)](#setDataBarRenderMode-int-) | Representerar läget för hur DataBar renderas när Excel-filer konverteras till html-filer. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Ange standardteckensnittets namn för export av html, standardteckensnittet kommer att användas när stilens teckensnitt inte finns, om detta egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null. |
| [setDisableCss(boolean value)](#setDisableCss-boolean-) | Anger om endast inline-stilar ska tillämpas, utan att förlita sig på CSS. |
| [setDisableDownlevelRevealedComments(boolean value)](#setDisableDownlevelRevealedComments-boolean-) | Anger om Downlevel-revealed villkorliga kommentarer ska inaktiveras vid export av fil till html, standardvärdet är false. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Ställer in typen av inbäddning av teckensnittsfilen i html‑filen. |
| [setEnableCssCustomProperties(boolean value)](#setEnableCssCustomProperties-boolean-) | Optimera html-utdata genom att använda anpassade CSS-egenskaper. |
| [setEncodeEntityAsCode(boolean value)](#setEncodeEntityAsCode-boolean-) | Anger om html-teckenentiteter ersätts med decimalkod. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Om inte angivet, använd Encoding.UTF8 som standardkodningstyp. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [setExcludeUnusedStyles(boolean value)](#setExcludeUnusedStyles-boolean-) | Anger om oanvända stilar ska uteslutas. |
| [setExpImageToTempDir(boolean value)](#setExpImageToTempDir-boolean-) | Anger om bildfiler ska exporteras till en temporär katalog. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Anger om endast det aktiva kalkylbladet ska exporteras till html-filen. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Ställer in exporten av CellArea för det aktuella aktiva kalkylbladet. |
| [setExportBogusRowData(boolean value)](#setExportBogusRowData-boolean-) | Anger om export av felaktiga data i den sista raden. |
| [setExportCellCoordinate(boolean value)](#setExportCellCoordinate-boolean-) | Anger om Excel-koordinater för icke tomma celler exporteras när filen sparas som HTML. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Anger om kommentarer exporteras när filen sparas till html, standardvärdet är falskt. |
| [setExportCommentsType(int value)](#setExportCommentsType-int-) | Representerar typ av export av kommentarer till HTML-filer. |
| [setExportDataOptions(int value)](#setExportDataOptions-int-) | Anger regeln för export av HTML-fildata. Standardvärdet är Alla. |
| [setExportDocumentProperties(boolean value)](#setExportDocumentProperties-boolean-) | Anger om dokumentegenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet. |
| [setExportExtraHeadings(boolean value)](#setExportExtraHeadings-boolean-) | Anger om extra rubriker exporteras när textens längd överstiger maximal visningskolumn. |
| [setExportFormula(boolean value)](#setExportFormula-boolean-) | Anger om formler exporteras när filen sparas som HTML. |
| [setExportFrameScriptsAndProperties(boolean value)](#setExportFrameScriptsAndProperties-boolean-) | Anger om ramskript och dokumentegenskaper exporteras. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Anger om rutnätslinjer exporteras. Standardvärdet är false. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Anger om bladets rad- och kolumnrubriker exporteras när du sparar till HTML-filer. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Anger om dolt kalkylbladsinnehåll exporteras. Standardvärdet är true. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB. |
| [setExportNamedRangeAnchors(boolean value)](#setExportNamedRangeAnchors-boolean-) | Anger om ankarelement för namngivna områden exporteras när du sparar som HTML. |
| [setExportObjectListener(IExportObjectListener value)](#setExportObjectListener-com.aspose.cells.IExportObjectListener-) | Ställer in ExportObjectListener för export av objekt. |
| [setExportPageFooters(boolean value)](#setExportPageFooters-boolean-) | Anger om sidhuvuden exporteras. |
| [setExportPageHeaders(boolean value)](#setExportPageHeaders-boolean-) | Anger om sidhuvuden exporteras. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Anger om endast utskriftsområdet exporteras till HTML-filen. |
| [setExportRowColumnHeadings(boolean value)](#setExportRowColumnHeadings-boolean-) | Anger om bladets rad- och kolumnrubriker exporteras när du sparar till HTML-filer. |
| [setExportSimilarBorderStyle(boolean value)](#setExportSimilarBorderStyle-boolean-) | Anger om liknande kantlinjestil exporteras när kantlinjestilen inte stöds av webbläsare. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Anger om den enda fliken exporteras när filen bara har ett kalkylblad. |
| [setExportWorkbookProperties(boolean value)](#setExportWorkbookProperties-boolean-) | Anger om arbetsboks egenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet. |
| [setExportWorksheetCSSSeparately(boolean value)](#setExportWorksheetCSSSeparately-boolean-) | Anger om kalkylbladets CSS exporteras separat. Standardvärdet är false. |
| [setExportWorksheetProperties(boolean value)](#setExportWorksheetProperties-boolean-) | Anger om kalkylblads egenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet. |
| [setFilePathProvider(IFilePathProvider value)](#setFilePathProvider-com.aspose.cells.IFilePathProvider-) | Ställer in IFilePathProvider för separat export av kalkylblad till html. |
| [setFormatDataIgnoreColumnWidth(boolean value)](#setFormatDataIgnoreColumnWidth-boolean-) | Anger om hela formaterade celldata visas när den överskrider kolumnen. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | Anger om fullständig sökvägslänk används i sheet00x.htm, filelist.xml och tabstrip.htm. |
| [setHiddenColDisplayType(int value)](#setHiddenColDisplayType-int-) | Dold kolumn (bredden på denna kolumn är 0) i Excel, innan du sparar detta i HTML-format, om HtmlHiddenColDisplayType är "Remove" kommer den dolda kolumnen inte att skrivas ut, om värdet är "Hidden" kommer kolumnen att skrivas ut men vara dold, standardvärdet är "Hidden". |
| [setHiddenRowDisplayType(int value)](#setHiddenRowDisplayType-int-) | Dold rad (höjden på den här raden är 0) i excel, innan du sparar detta i html-format, om HtmlHiddenRowDisplayType är "Remove" så kommer den dolda raden inte att skrivas ut, om värdet är "Hidden" så kommer raden att skrivas ut men vara dold, standardvärdet är "Hidden". |
| [setHideOverflowWrappedText(boolean value)](#setHideOverflowWrappedText-boolean-) | Anger om överskjutande text ska döljas när cellformatet är inställt på radbrytning. |
| [setHtmlCrossStringType(int value)](#setHtmlCrossStringType-int-) | Anger om en sträng som sträcker sig över flera celler ska visas på samma sätt som i MS Excel när en Excel-fil sparas i html-format. |
| [setHtmlVersion(int value)](#setHtmlVersion-int-) | Specificerar version av HTML-standarden som ska användas när HTML-formatet sparas. |
| [setIECompatible(boolean value)](#setIECompatible-boolean-) | Anger om den genererade HTML är kompatibel med IE‑webbläsaren. |
| [setIgnoreInvisibleShapes(boolean value)](#setIgnoreInvisibleShapes-boolean-) | Anger om osynliga former ska exporteras. |
| [setImageScalable(boolean value)](#setImageScalable-boolean-) | Anger om skalbar enhet ska användas för att beskriva bildens bredd när skalbar enhet används för att beskriva kolumnens bredd. |
| [setJsBrowserCompatible(boolean value)](#setJsBrowserCompatible-boolean-) | Anger om JavaScript är kompatibel med webbläsare som inte stödjer JavaScript. |
| [setLayoutMode(int value)](#setLayoutMode-int-) | Ställer in layoutläget när du sparar till HTML. |
| [setLinkTargetType(int value)](#setLinkTargetType-int-) | Anger typen av target-attribut i `<a>`-länk. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [setMergeEmptyTdForcely(boolean value)](#setMergeEmptyTdForcely-boolean-) | Anger om tomma TD-element ska slås ihop tvångsmässigt vid export av fil till html. |
| [setMergeEmptyTdType(int value)](#setMergeEmptyTdType-int-) | Alternativet för att slå ihop intilliggande tomma celler (tomma td-element). Standardvärdet är MergeEmptyTdType.Default. |
| [setMobileCompatible(boolean value)](#setMobileCompatible-boolean-) | Anger om den genererade HTML är kompatibel med mobila enheter. |
| [setOfficeMathOutputMode(int value)](#setOfficeMathOutputMode-int-) | Anger hur OfficeMath-objekt exporteras till HTML, standardvärdet är Image. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | Titeln på html-sidan. |
| [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Anger om html-taggar (såsom `<div></div>`) i cellen ska tolkas som cellvärde eller bevaras som de är. |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Anger om html- eller mht-fil är presentationspreferens. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Anger om den senaste diagramdata ska cachas. |
| [setSaveAsSingleFile(boolean value)](#setSaveAsSingleFile-boolean-) | Anger om html ska sparas som en enda fil. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Ställer in vilka blad som ska renderas. |
| [setShowAllSheets(boolean value)](#setShowAllSheets-boolean-) | Anger om alla blad ska visas när du sparar som en enda html-fil. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Anger om definierade namn ska sorteras innan filen sparas. |
| [setSpaceMode(int value)](#setSpaceMode-int-) | Anger hur mellanslag renderas i HTML-utdata. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Ställer in IStreamProvider för export av objekt. |
| [setTableCssId(String value)](#setTableCssId-java.lang.String-) | Ställer in prefixet för typ‑css‑namnet, t.ex. tr, col, td osv., som finns i tabell‑elementet med det specifika TableCssId‑attributet. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Anger om inställning för SmartArt ska uppdateras. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Ställer in varningsåteranrop. |
| [setWidthScalable(boolean value)](#setWidthScalable-boolean-) | Anger om kolumnbredd ska exporteras i skalanhet till html. |
| [setWorksheetScalable(boolean value)](#setWorksheetScalable-boolean-) | Anger om html ska zoomas in eller ut via arbetsbladets zoomnivå när filen sparas till html, standardvärdet är false. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Skapar alternativ för att spara en html-fil.

### HtmlSaveOptions(int saveFormat) {#HtmlSaveOptions-int-}
```
public HtmlSaveOptions(int saveFormat)
```


Skapar alternativ för att spara en htm-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Filformatet. Det bör vara någon av följande typer: [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML) eller [SaveFormat.M\_HTML](../../com.aspose.cells/saveformat\#M-HTML), annars kommer det sparade formatet automatiskt att sättas till [SaveFormat.HTML](../../com.aspose.cells/saveformat\#HTML). |

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
### getAddGenericFont() {#getAddGenericFont--}
```
public boolean getAddGenericFont()
```


Anger om ett generiskt teckensnitt ska läggas till i CSS font-family. Standardvärdet är true.

**Returns:**
boolean
### getAddTooltipText() {#getAddTooltipText--}
```
public boolean getAddTooltipText()
```


Anger om verktygstips ska läggas till när data inte kan visas helt. Standardvärdet är false.

**Returns:**
boolean
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Katalogen där de bifogade filerna kommer att sparas. Endast för att spara till html‑ström.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Ange Url‑prefixet för bifogade filer, t.ex. bild i html‑filen. Endast för att spara till html‑ström.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Mappen för temporära filer som kan användas som datacache.

**Remarks**

Om mappen inte har specificerats är standardvärdet för den [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Om dess standardvärde är null eller tomt, eller har specificerats som null eller tomt, kommer ingen cachefil att användas när arbetsboken sparas.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Anger om formler ska beräknas innan html-filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getCellCssPrefix() {#getCellCssPrefix--}
```
public String getCellCssPrefix()
```


Hämtar prefixet för css-namnet, standardvärdet är "".

**Returns:**
java.lang.String
### getCellNameAttribute() {#getCellNameAttribute--}
```
public String getCellNameAttribute()
```


Specificerar attributet som anger CellName att skrivas. (t.ex. Om värdet är "id", så blir utdata för cell "A1": <td id='A1'>). Standardvärdet är null.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Om kontroll av begränsningar i Excel-filen när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32K. När du anger ett värde som är längre än 32K trunkeras det.

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


Gör arbetsboken tom efter att filen har sparats.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getCssStyles() {#getCssStyles--}
```
public String getCssStyles()
```


Hämtar de ytterligare css‑stilarna för formateraren. Fungerar endast när [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) är True.  CssStyles="body \{ padding: 5px \}";

**Returns:**
java.lang.String
### getDataBarRenderMode() {#getDataBarRenderMode--}
```
public int getDataBarRenderMode()
```


Representerar läget för hur DataBar renderas när Excel‑filer konverteras till html‑filer. Standardvärdet är [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

Se [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Ange standardteckensnittets namn för export av html, standardteckensnittet kommer att användas när stilens teckensnitt inte finns, om detta egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null.

**Returns:**
java.lang.String
### getDisableCss() {#getDisableCss--}
```
public boolean getDisableCss()
```


Anger om endast inline‑stilar ska tillämpas, utan att förlita sig på CSS. Standardvärdet är false.

**Returns:**
boolean
### getDisableDownlevelRevealedComments() {#getDisableDownlevelRevealedComments--}
```
public boolean getDisableDownlevelRevealedComments()
```


Anger om Downlevel-revealed villkorliga kommentarer ska inaktiveras vid export av fil till html, standardvärdet är false.

**Returns:**
boolean
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```


Hämtar typen av inbäddad teckensnittfil i html-filen. Standardvärdet är [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) vilket indikerar att inget teckensnitt kommer att bäddas in i html.

Se [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Returns:**
int
### getEnableCssCustomProperties() {#getEnableCssCustomProperties--}
```
public boolean getEnableCssCustomProperties()
```


Optimera html-utdata genom att använda anpassade CSS-egenskaper. Till exempel, i scenariot där det finns flera förekomster av en base64-bild, krävs bilddata endast sparas en gång med en anpassad egenskap, så att prestandan för den resulterande html kan förbättras. Standardvärdet är falskt.

**Returns:**
boolean
### getEncodeEntityAsCode() {#getEncodeEntityAsCode--}
```
public boolean getEncodeEntityAsCode()
```


Anger om html-teckenentiteter ersätts med decimalkod. (t.ex. "&nbsp;" ersätts med "&\#160;"). Standardvärdet är falskt.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Om inte angivet, använd Encoding.UTF8 som standardkodningstyp.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Anger om dokumentegenskaper ska krypteras vid sparande som .xls-fil. Standardvärdet är sant.

**Remarks**

Endast för .xls, .xlsx, .xlsb och .xlsm-filer.

**Returns:**
boolean
### getExcludeUnusedStyles() {#getExcludeUnusedStyles--}
```
public boolean getExcludeUnusedStyles()
```


Anger om oanvända stilar exkluderas. För de genererade html-filerna kan uteslutning av oanvända stilar göra filstorleken mindre utan att påverka de visuella effekterna. Så standardvärdet för denna egenskap är true. Om användaren behöver behålla alla stilar i arbetsboken för den genererade html (t.ex. i scenariot där användaren senare behöver återställa arbetsboken från den genererade html), sätt denna egenskap till false.

**Returns:**
boolean
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Anger om endast den aktiva arbetsbladet exporteras till html-fil. Om true exporteras endast det aktiva arbetsbladet till html-fil; om false exporteras hela arbetsboken till html-fil. Standardvärdet är false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Hämtar exportområdet CellArea för det aktuella aktiva arbetsbladet. Om du anger detta attribut kommer utskriftsområdet för det aktuella aktiva arbetsbladet att utelämnas. Endast det specificerade området exporteras när filen sparas som html.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportBogusRowData() {#getExportBogusRowData--}
```
public boolean getExportBogusRowData()
```


Anger om felaktig data för den sista raden exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet.

**Returns:**
boolean
### getExportCellCoordinate() {#getExportCellCoordinate--}
```
public boolean getExportCellCoordinate()
```


Anger om Excel-koordinater för icke-tomma celler exporteras när filen sparas som html. Standardvärdet är false. Om du vill importera den genererade html till Excel, behåll standardvärdet.

**Returns:**
boolean
### getExportCommentsType() {#getExportCommentsType--}
```
public int getExportCommentsType()
```


Representerar typ av export av kommentarer till HTML-filer.

Se [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Returns:**
int
### getExportDataOptions() {#getExportDataOptions--}
```
public int getExportDataOptions()
```


Anger regeln för export av HTML-fildata. Standardvärdet är Alla.

Se [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Returns:**
int
### getExportDocumentProperties() {#getExportDocumentProperties--}
```
public boolean getExportDocumentProperties()
```


Anger om dokumentegenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet.

**Returns:**
boolean
### getExportExtraHeadings() {#getExportExtraHeadings--}
```
public boolean getExportExtraHeadings()
```


Anger om extra rubriker exporteras när textlängden är längre än den maximala visningskolumnen. Standardvärdet är false. Om du vill importera html-filen till Excel, behåll standardvärdet.

**Returns:**
boolean
### getExportFormula() {#getExportFormula--}
```
public boolean getExportFormula()
```


Anger om formler exporteras när filen sparas som html. Standardvärdet är true. Om du vill importera den genererade html till Excel, behåll standardvärdet.

**Returns:**
boolean
### getExportFrameScriptsAndProperties() {#getExportFrameScriptsAndProperties--}
```
public boolean getExportFrameScriptsAndProperties()
```


Anger om ram‑skript och dokumentegenskaper exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet.

**Returns:**
boolean
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Anger om rutnätslinjer exporteras. Standardvärdet är false.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Anger om bladets rad- och kolumnrubriker exporteras när du sparar till HTML-filer.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen HtmlSaveOptions.ExportRowColumnHeadings. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Anger om dolt kalkylbladsinnehåll exporteras. Standardvärdet är true.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB.

**Remarks**

När denna egenskap är satt till true exporteras bilddata direkt i img-elementen och separata filer skapas inte.

**Returns:**
boolean
### getExportNamedRangeAnchors() {#getExportNamedRangeAnchors--}
```
public boolean getExportNamedRangeAnchors()
```


Anger om ankarelement för namngivna områden ska exporteras när du sparar som HTML. Standardvärdet är true.

**Returns:**
boolean
### getExportObjectListener() {#getExportObjectListener--}
```
public IExportObjectListener getExportObjectListener()
```


Hämtar ExportObjectListener för export av objekt.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen HtmlSaveOptions.IStreamProvider. Denna egenskap kommer att tas bort 12 månader senare sedan augusti 2015. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[IExportObjectListener](../../com.aspose.cells/iexportobjectlistener)
### getExportPageFooters() {#getExportPageFooters--}
```
public boolean getExportPageFooters()
```


Anger om sidhuvuden exporteras.

**Remarks**

Fungerar endast när [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) är True.

**Returns:**
boolean
### getExportPageHeaders() {#getExportPageHeaders--}
```
public boolean getExportPageHeaders()
```


Anger om sidhuvuden exporteras.

**Remarks**

Fungerar endast när [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) är True.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Anger om endast utskriftsområdet ska exporteras till html‑fil. Standardvärdet är false.

**Returns:**
boolean
### getExportRowColumnHeadings() {#getExportRowColumnHeadings--}
```
public boolean getExportRowColumnHeadings()
```


Anger om bladets rad- och kolumnrubriker exporteras när du sparar till HTML-filer.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getExportSimilarBorderStyle() {#getExportSimilarBorderStyle--}
```
public boolean getExportSimilarBorderStyle()
```


Anger om en liknande kantstil ska exporteras när kantstilen inte stöds av webbläsare. Om du vill importera html‑ eller mht‑filen till Excel, behåll standardvärdet. Standardvärdet är false.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Anger om den enda fliken ska exporteras när filen bara har ett arbetsblad. Standardvärdet är false.

**Returns:**
boolean
### getExportWorkbookProperties() {#getExportWorkbookProperties--}
```
public boolean getExportWorkbookProperties()
```


Anger om arbetsboks egenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet.

**Returns:**
boolean
### getExportWorksheetCSSSeparately() {#getExportWorksheetCSSSeparately--}
```
public boolean getExportWorksheetCSSSeparately()
```


Anger om kalkylbladets CSS exporteras separat. Standardvärdet är false.

**Returns:**
boolean
### getExportWorksheetProperties() {#getExportWorksheetProperties--}
```
public boolean getExportWorksheetProperties()
```


Anger om kalkylblads egenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet.

**Returns:**
boolean
### getFilePathProvider() {#getFilePathProvider--}
```
public IFilePathProvider getFilePathProvider()
```


Hämtar IFilePathProvider för separat export av kalkylblad till HTML.

**Returns:**
[IFilePathProvider](../../com.aspose.cells/ifilepathprovider)
### getFormatDataIgnoreColumnWidth() {#getFormatDataIgnoreColumnWidth--}
```
public boolean getFormatDataIgnoreColumnWidth()
```


Anger om hela formaterade celldata ska visas när den överskrider kolumnen. Om true ignoreras kolumnbredden och hela cellens data exporteras. Om false exporteras data på samma sätt som i Excel. Standardvärdet är false.

**Returns:**
boolean
### getHiddenColDisplayType() {#getHiddenColDisplayType--}
```
public int getHiddenColDisplayType()
```


Dold kolumn (bredden på denna kolumn är 0) i Excel, innan du sparar detta i HTML-format, om HtmlHiddenColDisplayType är "Remove" kommer den dolda kolumnen inte att skrivas ut, om värdet är "Hidden" kommer kolumnen att skrivas ut men vara dold, standardvärdet är "Hidden".

Se [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Returns:**
int
### getHiddenRowDisplayType() {#getHiddenRowDisplayType--}
```
public int getHiddenRowDisplayType()
```


Dold rad (höjden på den här raden är 0) i excel, innan du sparar detta i html-format, om HtmlHiddenRowDisplayType är "Remove" så kommer den dolda raden inte att skrivas ut, om värdet är "Hidden" så kommer raden att skrivas ut men vara dold, standardvärdet är "Hidden".

Se [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Returns:**
int
### getHideOverflowWrappedText() {#getHideOverflowWrappedText--}
```
public boolean getHideOverflowWrappedText()
```


Anger om överskjutande text ska döljas när cellformatet är inställt på radbrytning. Standardvärdet är false

**Returns:**
boolean
### getHtmlCrossStringType() {#getHtmlCrossStringType--}
```
public int getHtmlCrossStringType()
```


Anger om en sträng som sträcker sig över flera celler visas på samma sätt som i MS Excel när en Excel‑fil sparas i html‑format. Som standard är värdet Default, så för strängar som sträcker sig över celler är skillnaden mellan html‑filerna som skapas av Aspose.Cells och MS Excel liten. Men prestandan för att skapa stora html‑filer blir flera gånger snabbare om värdet sätts till Cross jämfört med att sätta det till Default eller Fit2Cell.

Se [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Returns:**
int
### getHtmlVersion() {#getHtmlVersion--}
```
public int getHtmlVersion()
```


Anger vilken version av HTML‑standarden som ska användas vid sparande av HTML‑formatet. Standardvärdet är HtmlVersion.Default.

Se [HtmlVersion](../../com.aspose.cells/htmlversion).

**Returns:**
int
### getIgnoreInvisibleShapes() {#getIgnoreInvisibleShapes--}
```
public boolean getIgnoreInvisibleShapes()
```


Anger om osynliga former ska exporteras.

**Remarks**

Standardvärdet är false.

**Returns:**
boolean
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Hämta ImageOrPrintOptions-objektet innan export.

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getImageScalable() {#getImageScalable--}
```
public boolean getImageScalable()
```


Anger om skalbar enhet ska användas för att beskriva bildens bredd när skalbar enhet används för att beskriva kolumnbredden. Standardvärdet är true.

**Returns:**
boolean
### getLayoutMode() {#getLayoutMode--}
```
public int getLayoutMode()
```


Hämtar layoutläget vid sparande till HTML. Standardvärdet är [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Se [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Returns:**
int
### getLinkTargetType() {#getLinkTargetType--}
```
public int getLinkTargetType()
```


Anger typen av target‑attribut i `<a>`‑länk. Standardvärdet är HtmlLinkTargetType.Parent.

Se [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Returns:**
int
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getMergeEmptyTdForcely() {#getMergeEmptyTdForcely--}
```
public boolean getMergeEmptyTdForcely()
```


Anger om tomma TD‑element ska slås ihop tvångsmässigt vid export av fil till html. Storleken på html‑filen minskar avsevärt när värdet sätts till true. Standardvärdet är false. Om du vill importera html‑filen till Excel eller exportera perfekta rutnätslinjer vid sparande till html, behåll standardvärdet.

**Returns:**
boolean
### getMergeEmptyTdType() {#getMergeEmptyTdType--}
```
public int getMergeEmptyTdType()
```


Alternativet för att slå ihop intilliggande tomma celler (tomma td-element). Standardvärdet är MergeEmptyTdType.Default.

Se [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Returns:**
int
### getOfficeMathOutputMode() {#getOfficeMathOutputMode--}
```
public int getOfficeMathOutputMode()
```


Anger hur OfficeMath-objekt exporteras till HTML, standardvärdet är Image.

Se [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Returns:**
int
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


Titeln på html‑sidan. Endast för sparande till html‑ström.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Anger om html‑taggar (såsom `<div></div>`) i en cell ska tolkas som cellvärde eller bevaras som de är. Standardvärdet är true.

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Anger om html- eller mht-fil är presentationspreferens. Standardvärdet är false. Om du vill ha en vackrare presentation, vänligen sätt värdet till true.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Anger om den senaste diagramdata ska cachas.

**Returns:**
boolean
### getSaveAsSingleFile() {#getSaveAsSingleFile--}
```
public boolean getSaveAsSingleFile()
```


Anger om html ska sparas som en enda fil. Standardvärdet är false.

**Remarks**

Om det finns flera arbetsblad eller andra nödvändiga resurser såsom bilder i arbetsboken, måste dessa arbetsblad och resurser vanligtvis sparas i separata filer. I vissa scenarier kan användaren behöva bara en resulterande fil för att underlätta överföring. I så fall kan användaren sätta denna egenskap till true.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Hämtar filformatet för sparning.

Se [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Hämtar de blad som ska renderas. Standard är alla synliga blad i arbetsboken: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getShowAllSheets() {#getShowAllSheets--}
```
public boolean getShowAllSheets()
```


Anger om alla blad ska visas när du sparar som en enda html-fil.

**Remarks**

Fungerar endast när [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) är True.

**Returns:**
boolean
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Anger om externa definierade namn ska sorteras innan filen sparas.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Anger om definierade namn ska sorteras innan filen sparas.

**Returns:**
boolean
### getSpaceMode() {#getSpaceMode--}
```
public int getSpaceMode()
```


Anger hur mellanslag renderas i HTML-utdata. Detta alternativ tillämpas för närvarande endast på numeriska format (t.ex. bokföringsformat). Standardvärdet är [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Se [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Returns:**
int
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Hämtar IStreamProvider för att exportera objekt.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getTableCssId() {#getTableCssId--}
```
public String getTableCssId()
```


Hämtar prefixet för typens css-namn såsom tr, col, td osv., de finns i tabell‑elementet som har det specifika TableCssId‑attributet. Standardvärdet är "".

**Returns:**
java.lang.String
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Anger om inställning för SmartArt ska uppdateras. Standardvärdet är falskt.

**Remarks**

Påverkar endast efter att ha anropat metoden Shape.GetResultOfSmartArt() och de cachade formerna finns i mallfilen.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Anger om sammanslagna celler ska valideras innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Hämtar varningsåteranrop.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWidthScalable() {#getWidthScalable--}
```
public boolean getWidthScalable()
```


Anger om kolumnbredd exporteras i skalenhet till html. Standardvärdet är false.

**Returns:**
boolean
### getWorksheetScalable() {#getWorksheetScalable--}
```
public boolean getWorksheetScalable()
```


Anger om html ska zoomas in eller ut via arbetsbladets zoomnivå när filen sparas till html, standardvärdet är false.

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


Anger om tabellramarna är kollapsade. Standardvärdet är true.

**Returns:**
boolean
### isExpImageToTempDir() {#isExpImageToTempDir--}
```
public boolean isExpImageToTempDir()
```


Anger om bildfiler exporteras till en temporär katalog. Endast för att spara till html‑ström.

**Returns:**
boolean
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Anger om kommentarer exporteras när filen sparas till html, standardvärdet är falskt.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


Anger om fullständig sökvägslänk används i sheet00x.htm, filelist.xml och tabstrip.htm. Standardvärdet är false.

**Returns:**
boolean
### isIECompatible() {#isIECompatible--}
```
public boolean isIECompatible()
```


Anger om den genererade HTML är kompatibel med IE‑webbläsaren. Standardvärdet är false

**Returns:**
boolean
### isJsBrowserCompatible() {#isJsBrowserCompatible--}
```
public boolean isJsBrowserCompatible()
```


Anger om JavaScript är kompatibel med webbläsare som inte stödjer JavaScript. Standardvärdet är true.

**Returns:**
boolean
### isMobileCompatible() {#isMobileCompatible--}
```
public boolean isMobileCompatible()
```


Anger om den genererade HTML är kompatibel med mobila enheter. Standardvärdet är false.

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


Anger om ett generiskt teckensnitt ska läggas till i CSS font-family. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAddTooltipText(boolean value) {#setAddTooltipText-boolean-}
```
public void setAddTooltipText(boolean value)
```


Anger om verktygstips ska läggas till när data inte kan visas helt. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Katalogen där de bifogade filerna kommer att sparas. Endast för att spara till html‑ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Ange Url‑prefixet för bifogade filer, t.ex. bild i html‑filen. Endast för att spara till html‑ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setBorderCollapsed(boolean value) {#setBorderCollapsed-boolean-}
```
public void setBorderCollapsed(boolean value)
```


Anger om tabellramarna är kollapsade. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Mappen för temporära filer som kan användas som datacache.

**Remarks**

Om mappen inte har specificerats är standardvärdet för den [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Om dess standardvärde är null eller tomt, eller har specificerats som null eller tomt, kommer ingen cachefil att användas när arbetsboken sparas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Anger om formler ska beräknas innan html-filen sparas.

**Remarks**

Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCellCssPrefix(String value) {#setCellCssPrefix-java.lang.String-}
```
public void setCellCssPrefix(String value)
```


Ställer in prefixet för css‑namnet, standardvärdet är "".

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCellNameAttribute(String value) {#setCellNameAttribute-java.lang.String-}
```
public void setCellNameAttribute(String value)
```


Specificerar attributet som anger CellName att skrivas. (t.ex. Om värdet är "id", så blir utdata för cell "A1": <td id='A1'>). Standardvärdet är null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Om kontroll av begränsningar i Excel-filen när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32K. När du anger ett värde som är längre än 32K trunkeras det.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Gör arbetsboken tom efter att filen har sparats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCssStyles(String value) {#setCssStyles-java.lang.String-}
```
public void setCssStyles(String value)
```


Ställer in ytterligare css‑stilar för formateraren. Fungerar endast när [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) är True.  CssStyles="body \{ padding: 5px \}";

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDataBarRenderMode(int value) {#setDataBarRenderMode-int-}
```
public void setDataBarRenderMode(int value)
```


Representerar läget för hur DataBar renderas när Excel‑filer konverteras till html‑filer. Standardvärdet är [DataBarRenderMode.BACKGROUND\_COLOR](../../com.aspose.cells/databarrendermode\#BACKGROUND-COLOR).

Se [DataBarRenderMode](../../com.aspose.cells/databarrendermode).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Ange standardteckensnittets namn för export av html, standardteckensnittet kommer att användas när stilens teckensnitt inte finns, om detta egenskap är null kommer Aspose.Cells att använda ett universellt teckensnitt som har samma familj som originalteckensnittet, standardvärdet är null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDisableCss(boolean value) {#setDisableCss-boolean-}
```
public void setDisableCss(boolean value)
```


Anger om endast inline‑stilar ska tillämpas, utan att förlita sig på CSS. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDisableDownlevelRevealedComments(boolean value) {#setDisableDownlevelRevealedComments-boolean-}
```
public void setDisableDownlevelRevealedComments(boolean value)
```


Anger om Downlevel-revealed villkorliga kommentarer ska inaktiveras vid export av fil till html, standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```


Ställer in typen av inbäddning av teckensnittsfiler i html‑filen. Standardvärdet är [HtmlEmbeddedFontType.NONE](../../com.aspose.cells/htmlembeddedfonttype\#NONE) vilket indikerar att inget teckensnitt kommer att bäddas in i html.

Se [HtmlEmbeddedFontType](../../com.aspose.cells/htmlembeddedfonttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEnableCssCustomProperties(boolean value) {#setEnableCssCustomProperties-boolean-}
```
public void setEnableCssCustomProperties(boolean value)
```


Optimera html-utdata genom att använda anpassade CSS-egenskaper. Till exempel, i scenariot där det finns flera förekomster av en base64-bild, krävs bilddata endast sparas en gång med en anpassad egenskap, så att prestandan för den resulterande html kan förbättras. Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEncodeEntityAsCode(boolean value) {#setEncodeEntityAsCode-boolean-}
```
public void setEncodeEntityAsCode(boolean value)
```


Anger om html-teckenentiteter ersätts med decimalkod. (t.ex. "&nbsp;" ersätts med "&\#160;"). Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Om inte angivet, använd Encoding.UTF8 som standardkodningstyp.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```


Anger om dokumentegenskaper ska krypteras vid sparande som .xls-fil. Standardvärdet är sant.

**Remarks**

Endast för .xls, .xlsx, .xlsb och .xlsm-filer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExcludeUnusedStyles(boolean value) {#setExcludeUnusedStyles-boolean-}
```
public void setExcludeUnusedStyles(boolean value)
```


Anger om oanvända stilar exkluderas. För de genererade html-filerna kan uteslutning av oanvända stilar göra filstorleken mindre utan att påverka de visuella effekterna. Så standardvärdet för denna egenskap är true. Om användaren behöver behålla alla stilar i arbetsboken för den genererade html (t.ex. i scenariot där användaren senare behöver återställa arbetsboken från den genererade html), sätt denna egenskap till false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExpImageToTempDir(boolean value) {#setExpImageToTempDir-boolean-}
```
public void setExpImageToTempDir(boolean value)
```


Anger om bildfiler exporteras till en temporär katalog. Endast för att spara till html‑ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Anger om endast den aktiva arbetsbladet exporteras till html-fil. Om true exporteras endast det aktiva arbetsbladet till html-fil; om false exporteras hela arbetsboken till html-fil. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Ställer in export av CellArea för det aktuella aktiva arbetsbladet. Om du anger detta attribut kommer utskriftsområdet för det aktuella aktiva arbetsbladet att utelämnas. Endast det angivna området exporteras när filen sparas till html.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportBogusRowData(boolean value) {#setExportBogusRowData-boolean-}
```
public void setExportBogusRowData(boolean value)
```


Anger om felaktig data för den sista raden exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportCellCoordinate(boolean value) {#setExportCellCoordinate-boolean-}
```
public void setExportCellCoordinate(boolean value)
```


Anger om Excel-koordinater för icke-tomma celler exporteras när filen sparas som html. Standardvärdet är false. Om du vill importera den genererade html till Excel, behåll standardvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Anger om kommentarer exporteras när filen sparas till html, standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportCommentsType(int value) {#setExportCommentsType-int-}
```
public void setExportCommentsType(int value)
```


Representerar typ av export av kommentarer till HTML-filer.

Se [PrintCommentsType](../../com.aspose.cells/printcommentstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setExportDataOptions(int value) {#setExportDataOptions-int-}
```
public void setExportDataOptions(int value)
```


Anger regeln för export av HTML-fildata. Standardvärdet är Alla.

Se [HtmlExportDataOptions](../../com.aspose.cells/htmlexportdataoptions).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setExportDocumentProperties(boolean value) {#setExportDocumentProperties-boolean-}
```
public void setExportDocumentProperties(boolean value)
```


Anger om dokumentegenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportExtraHeadings(boolean value) {#setExportExtraHeadings-boolean-}
```
public void setExportExtraHeadings(boolean value)
```


Anger om extra rubriker exporteras när textlängden är längre än den maximala visningskolumnen. Standardvärdet är false. Om du vill importera html-filen till Excel, behåll standardvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportFormula(boolean value) {#setExportFormula-boolean-}
```
public void setExportFormula(boolean value)
```


Anger om formler exporteras när filen sparas som html. Standardvärdet är true. Om du vill importera den genererade html till Excel, behåll standardvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportFrameScriptsAndProperties(boolean value) {#setExportFrameScriptsAndProperties-boolean-}
```
public void setExportFrameScriptsAndProperties(boolean value)
```


Anger om ram‑skript och dokumentegenskaper exporteras. Standardvärdet är true. Om du vill importera html- eller mht-filen till Excel, behåll standardvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Anger om rutnätslinjer exporteras. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Anger om bladets rad- och kolumnrubriker exporteras när du sparar till HTML-filer.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen HtmlSaveOptions.ExportRowColumnHeadings. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Anger om dolt kalkylbladsinnehåll exporteras. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Anger om bilder sparas i Base64-format till HTML, MHTML eller EPUB.

**Remarks**

När denna egenskap är satt till true exporteras bilddata direkt i img-elementen och separata filer skapas inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportNamedRangeAnchors(boolean value) {#setExportNamedRangeAnchors-boolean-}
```
public void setExportNamedRangeAnchors(boolean value)
```


Anger om ankarelement för namngivna områden ska exporteras när du sparar som HTML. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportObjectListener(IExportObjectListener value) {#setExportObjectListener-com.aspose.cells.IExportObjectListener-}
```
public void setExportObjectListener(IExportObjectListener value)
```


Ställer in ExportObjectListener för export av objekt.

**Remarks**

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen HtmlSaveOptions.IStreamProvider. Denna egenskap kommer att tas bort 12 månader senare sedan augusti 2015. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IExportObjectListener](../../com.aspose.cells/iexportobjectlistener) |  |

### setExportPageFooters(boolean value) {#setExportPageFooters-boolean-}
```
public void setExportPageFooters(boolean value)
```


Anger om sidhuvuden exporteras.

**Remarks**

Fungerar endast när [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) är True.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportPageHeaders(boolean value) {#setExportPageHeaders-boolean-}
```
public void setExportPageHeaders(boolean value)
```


Anger om sidhuvuden exporteras.

**Remarks**

Fungerar endast när [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) är True.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Anger om endast utskriftsområdet ska exporteras till html‑fil. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportRowColumnHeadings(boolean value) {#setExportRowColumnHeadings-boolean-}
```
public void setExportRowColumnHeadings(boolean value)
```


Anger om bladets rad- och kolumnrubriker exporteras när du sparar till HTML-filer.

**Remarks**

Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportSimilarBorderStyle(boolean value) {#setExportSimilarBorderStyle-boolean-}
```
public void setExportSimilarBorderStyle(boolean value)
```


Anger om en liknande kantstil ska exporteras när kantstilen inte stöds av webbläsare. Om du vill importera html‑ eller mht‑filen till Excel, behåll standardvärdet. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Anger om den enda fliken ska exporteras när filen bara har ett arbetsblad. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportWorkbookProperties(boolean value) {#setExportWorkbookProperties-boolean-}
```
public void setExportWorkbookProperties(boolean value)
```


Anger om arbetsboks egenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportWorksheetCSSSeparately(boolean value) {#setExportWorksheetCSSSeparately-boolean-}
```
public void setExportWorksheetCSSSeparately(boolean value)
```


Anger om kalkylbladets CSS exporteras separat. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setExportWorksheetProperties(boolean value) {#setExportWorksheetProperties-boolean-}
```
public void setExportWorksheetProperties(boolean value)
```


Anger om kalkylblads egenskaper exporteras. Standardvärdet är true. Om du vill importera HTML- eller MHT-filen till Excel, behåll standardvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFilePathProvider(IFilePathProvider value) {#setFilePathProvider-com.aspose.cells.IFilePathProvider-}
```
public void setFilePathProvider(IFilePathProvider value)
```


Ställer in IFilePathProvider för separat export av kalkylblad till html.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IFilePathProvider](../../com.aspose.cells/ifilepathprovider) |  |

### setFormatDataIgnoreColumnWidth(boolean value) {#setFormatDataIgnoreColumnWidth-boolean-}
```
public void setFormatDataIgnoreColumnWidth(boolean value)
```


Anger om hela formaterade celldata ska visas när den överskrider kolumnen. Om true ignoreras kolumnbredden och hela cellens data exporteras. Om false exporteras data på samma sätt som i Excel. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


Anger om fullständig sökvägslänk används i sheet00x.htm, filelist.xml och tabstrip.htm. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHiddenColDisplayType(int value) {#setHiddenColDisplayType-int-}
```
public void setHiddenColDisplayType(int value)
```


Dold kolumn (bredden på denna kolumn är 0) i Excel, innan du sparar detta i HTML-format, om HtmlHiddenColDisplayType är "Remove" kommer den dolda kolumnen inte att skrivas ut, om värdet är "Hidden" kommer kolumnen att skrivas ut men vara dold, standardvärdet är "Hidden".

Se [HtmlHiddenColDisplayType](../../com.aspose.cells/htmlhiddencoldisplaytype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHiddenRowDisplayType(int value) {#setHiddenRowDisplayType-int-}
```
public void setHiddenRowDisplayType(int value)
```


Dold rad (höjden på den här raden är 0) i excel, innan du sparar detta i html-format, om HtmlHiddenRowDisplayType är "Remove" så kommer den dolda raden inte att skrivas ut, om värdet är "Hidden" så kommer raden att skrivas ut men vara dold, standardvärdet är "Hidden".

Se [HtmlHiddenRowDisplayType](../../com.aspose.cells/htmlhiddenrowdisplaytype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHideOverflowWrappedText(boolean value) {#setHideOverflowWrappedText-boolean-}
```
public void setHideOverflowWrappedText(boolean value)
```


Anger om överskjutande text ska döljas när cellformatet är inställt på radbrytning. Standardvärdet är false

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHtmlCrossStringType(int value) {#setHtmlCrossStringType-int-}
```
public void setHtmlCrossStringType(int value)
```


Anger om en sträng som sträcker sig över flera celler visas på samma sätt som i MS Excel när en Excel‑fil sparas i html‑format. Som standard är värdet Default, så för strängar som sträcker sig över celler är skillnaden mellan html‑filerna som skapas av Aspose.Cells och MS Excel liten. Men prestandan för att skapa stora html‑filer blir flera gånger snabbare om värdet sätts till Cross jämfört med att sätta det till Default eller Fit2Cell.

Se [HtmlCrossType](../../com.aspose.cells/htmlcrosstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHtmlVersion(int value) {#setHtmlVersion-int-}
```
public void setHtmlVersion(int value)
```


Anger vilken version av HTML‑standarden som ska användas vid sparande av HTML‑formatet. Standardvärdet är HtmlVersion.Default.

Se [HtmlVersion](../../com.aspose.cells/htmlversion).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setIECompatible(boolean value) {#setIECompatible-boolean-}
```
public void setIECompatible(boolean value)
```


Anger om den genererade HTML är kompatibel med IE‑webbläsaren. Standardvärdet är false

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setIgnoreInvisibleShapes(boolean value) {#setIgnoreInvisibleShapes-boolean-}
```
public void setIgnoreInvisibleShapes(boolean value)
```


Anger om osynliga former ska exporteras.

**Remarks**

Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setImageScalable(boolean value) {#setImageScalable-boolean-}
```
public void setImageScalable(boolean value)
```


Anger om skalbar enhet ska användas för att beskriva bildens bredd när skalbar enhet används för att beskriva kolumnbredden. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setJsBrowserCompatible(boolean value) {#setJsBrowserCompatible-boolean-}
```
public void setJsBrowserCompatible(boolean value)
```


Anger om JavaScript är kompatibel med webbläsare som inte stödjer JavaScript. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLayoutMode(int value) {#setLayoutMode-int-}
```
public void setLayoutMode(int value)
```


Ställer in layoutläge vid sparande till HTML. Standardvärdet är [HtmlLayoutMode.NORMAL](../../com.aspose.cells/htmllayoutmode\#NORMAL)

Se [HtmlLayoutMode](../../com.aspose.cells/htmllayoutmode).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLinkTargetType(int value) {#setLinkTargetType-int-}
```
public void setLinkTargetType(int value)
```


Anger typen av target‑attribut i `<a>`‑länk. Standardvärdet är HtmlLinkTargetType.Parent.

Se [HtmlLinkTargetType](../../com.aspose.cells/htmllinktargettype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMergeEmptyTdForcely(boolean value) {#setMergeEmptyTdForcely-boolean-}
```
public void setMergeEmptyTdForcely(boolean value)
```


Anger om tomma TD‑element ska slås ihop tvångsmässigt vid export av fil till html. Storleken på html‑filen minskar avsevärt när värdet sätts till true. Standardvärdet är false. Om du vill importera html‑filen till Excel eller exportera perfekta rutnätslinjer vid sparande till html, behåll standardvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setMergeEmptyTdType(int value) {#setMergeEmptyTdType-int-}
```
public void setMergeEmptyTdType(int value)
```


Alternativet för att slå ihop intilliggande tomma celler (tomma td-element). Standardvärdet är MergeEmptyTdType.Default.

Se [MergeEmptyTdType](../../com.aspose.cells/mergeemptytdtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMobileCompatible(boolean value) {#setMobileCompatible-boolean-}
```
public void setMobileCompatible(boolean value)
```


Anger om den genererade HTML är kompatibel med mobila enheter. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOfficeMathOutputMode(int value) {#setOfficeMathOutputMode-int-}
```
public void setOfficeMathOutputMode(int value)
```


Anger hur OfficeMath-objekt exporteras till HTML, standardvärdet är Image.

Se [HtmlOfficeMathOutputType](../../com.aspose.cells/htmlofficemathoutputtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


Titeln på html‑sidan. Endast för sparande till html‑ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Anger om html‑taggar (såsom `<div></div>`) i en cell ska tolkas som cellvärde eller bevaras som de är. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Anger om html- eller mht-fil är presentationspreferens. Standardvärdet är false. Om du vill ha en vackrare presentation, vänligen sätt värdet till true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Anger om den senaste diagramdata ska cachas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSaveAsSingleFile(boolean value) {#setSaveAsSingleFile-boolean-}
```
public void setSaveAsSingleFile(boolean value)
```


Anger om html ska sparas som en enda fil. Standardvärdet är false.

**Remarks**

Om det finns flera arbetsblad eller andra nödvändiga resurser såsom bilder i arbetsboken, måste dessa arbetsblad och resurser vanligtvis sparas i separata filer. I vissa scenarier kan användaren behöva bara en resulterande fil för att underlätta överföring. I så fall kan användaren sätta denna egenskap till true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Ställer in de blad som ska renderas. Standard är alla synliga blad i arbetsboken: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setShowAllSheets(boolean value) {#setShowAllSheets-boolean-}
```
public void setShowAllSheets(boolean value)
```


Anger om alla blad ska visas när du sparar som en enda html-fil.

**Remarks**

Fungerar endast när [getSaveAsSingleFile()](../../com.aspose.cells/htmlsaveoptions\#getSaveAsSingleFile--) är True.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Anger om externa definierade namn ska sorteras innan filen sparas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Anger om definierade namn ska sorteras innan filen sparas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSpaceMode(int value) {#setSpaceMode-int-}
```
public void setSpaceMode(int value)
```


Anger hur mellanslag renderas i HTML-utdata. Detta alternativ tillämpas för närvarande endast på numeriska format (t.ex. bokföringsformat). Standardvärdet är [HtmlSpaceMode.CSS](../../com.aspose.cells/htmlspacemode\#CSS).

Se [HtmlSpaceMode](../../com.aspose.cells/htmlspacemode).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Ställer in IStreamProvider för export av objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setTableCssId(String value) {#setTableCssId-java.lang.String-}
```
public void setTableCssId(String value)
```


Ställer in prefixet för typens css‑namn såsom tr, col, td osv., de finns i tabell‑elementet som har det specifika TableCssId‑attributet. Standardvärdet är "".

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Anger om inställning för SmartArt ska uppdateras. Standardvärdet är falskt.

**Remarks**

Påverkar endast efter att ha anropat metoden Shape.GetResultOfSmartArt() och de cachade formerna finns i mallfilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Anger om sammanslagna celler ska valideras innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Ställer in varningsåteranrop.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setWidthScalable(boolean value) {#setWidthScalable-boolean-}
```
public void setWidthScalable(boolean value)
```


Anger om kolumnbredd exporteras i skalenhet till html. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setWorksheetScalable(boolean value) {#setWorksheetScalable-boolean-}
```
public void setWorksheetScalable(boolean value)
```


Anger om html ska zoomas in eller ut via arbetsbladets zoomnivå när filen sparas till html, standardvärdet är false.

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

