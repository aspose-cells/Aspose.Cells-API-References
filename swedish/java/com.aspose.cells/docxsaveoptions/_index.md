---
title: "DocxSaveOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativ för att spara .docx-fil."
type: docs
url: /sv/java/com.aspose.cells/docxsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class DocxSaveOptions extends PaginatedSaveOptions
```

Representerar alternativ för att spara .docx-fil.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [DocxSaveOptions()](#DocxSaveOptions--) | Representerar alternativ för att spara .docx-fil. |
| [DocxSaveOptions(boolean saveAsImage)](#DocxSaveOptions-boolean-) | Representerar alternativ för att spara .docx-fil. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [getAsFlatOpc()](#getAsFlatOpc--) | Anger om sparande som en flat opc-fil som kan genereras av Open XML SDK |
| [getAsNormalView()](#getAsNormalView--) | Exporterar Excel-fil till docx-fil i normal vy. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Mappen för temporära filer som kan användas som datacache. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Gör arbetsboken tom efter att filen har sparats. |
| [getCreateDirectory()](#getCreateDirectory--) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Hämtar anpassade inställningar under rendering. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Hämtar standardspråk för redigering. |
| [getDefaultFont()](#getDefaultFont--) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [getEmbedXlsxAsChartDataSource()](#getEmbedXlsxAsChartDataSource--) | Anger om en xlsx-fil ska bäddas in som datakälla för diagrammet. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Inställning för rendering av Emf-metafil. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [getGridlineColor()](#getGridlineColor--) | Hämtar färg på rutnätslinjer. |
| [getGridlineType()](#getGridlineType--) | Hämtar typ av rutnätslinje. |
| [getIgnoreError()](#getIgnoreError--) | Anger om du behöver dölja felet under rendering. |
| [getMergeAreas()](#getMergeAreas--) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [getPageCount()](#getPageCount--) | Hämtar antalet sidor som ska sparas. |
| [getPageIndex()](#getPageIndex--) | Hämtar det 0-baserade indexet för den första sidan som ska sparas. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Styr/indikera framsteg för sid sparningsprocessen. |
| [getPrintingPageType()](#getPrintingPageType--) | Anger vilka sidor som inte kommer att skrivas ut. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Anger om den senaste diagramdata ska cachas. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Hämtar de Excel-specifika renderingsbeteendena som ska tillämpas. |
| [getSaveAsEditableShapes()](#getSaveAsEditableShapes--) | Spara alla ritobjekt som redigerbara former i Word-filen, så att du kan redigera dem i Word. |
| [getSaveAsEditableShaps()](#getSaveAsEditableShaps--) | Spara alla ritobjekt som redigerbara former i Word-filen. Så kan du redigera dem i Word. |
| [getSaveElementType()](#getSaveElementType--) | Anger vilka element som ska sparas. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar filformatet för sparning. |
| [getSheetSet()](#getSheetSet--) | Hämtar bladen som ska renderas. |
| [getSortExternalNames()](#getSortExternalNames--) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [getSortNames()](#getSortNames--) | Anger om definierade namn ska sorteras innan filen sparas. |
| [getTextCrossType()](#getTextCrossType--) | Hämtar visningstyp för text när textbredden är större än cellbredden. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Anger om inställning för SmartArt ska uppdateras. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [getWarningCallback()](#getWarningCallback--) | Hämtar varningsåteranrop. |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [setAsFlatOpc(boolean value)](#setAsFlatOpc-boolean-) | Anger om sparande som en flat opc-fil som kan genereras av Open XML SDK |
| [setAsNormalView(boolean value)](#setAsNormalView-boolean-) | Exporterar Excel-fil till docx-fil i normal vy. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Mappen för temporära filer som kan användas som datacache. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [setClearData(boolean value)](#setClearData-boolean-) | Gör arbetsboken tom efter att filen har sparats. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Ställer in anpassade inställningar under rendering. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Ställer in standardspråk för redigering. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [setEmbedXlsxAsChartDataSource(boolean value)](#setEmbedXlsxAsChartDataSource-boolean-) | Anger om en xlsx-fil ska bäddas in som datakälla för diagrammet. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Inställning för rendering av Emf-metafil. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Ställer in färg för rutnätslinjer. |
| [setGridlineType(int value)](#setGridlineType-int-) | Ställer in typ för rutnätslinjer. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Anger om du behöver dölja felet under rendering. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [setPageCount(int value)](#setPageCount-int-) | Ställer in antalet sidor som ska sparas. |
| [setPageIndex(int value)](#setPageIndex-int-) | Ställer in det 0-baserade indexet för den första sidan som ska sparas. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Styr/indikera framsteg för sid sparningsprocessen. |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Anger vilka sidor som inte kommer att skrivas ut. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Anger om den senaste diagramdata ska cachas. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Ställer in de Excel-specifika renderingsbeteendena som ska tillämpas. |
| [setSaveAsEditableShapes(boolean value)](#setSaveAsEditableShapes-boolean-) | Spara alla ritobjekt som redigerbara former i Word-filen, så att du kan redigera dem i Word. |
| [setSaveAsEditableShaps(boolean value)](#setSaveAsEditableShaps-boolean-) | Spara alla ritobjekt som redigerbara former i Word-filen. Så kan du redigera dem i Word. |
| [setSaveElementType(int value)](#setSaveElementType-int-) | Anger vilka element som ska sparas. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Ställer in vilka blad som ska renderas. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Anger om definierade namn ska sorteras innan filen sparas. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Ställer in visningstyp för text när textbredden är större än cellbredden. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Anger om inställning för SmartArt ska uppdateras. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Ställer in varningsåteranrop. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DocxSaveOptions() {#DocxSaveOptions--}
```
public DocxSaveOptions()
```


Representerar alternativ för att spara .docx-fil.

### DocxSaveOptions(boolean saveAsImage) {#DocxSaveOptions-boolean-}
```
public DocxSaveOptions(boolean saveAsImage)
```


Representerar alternativ för att spara .docx-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveAsImage | boolean | Om True konverteras arbetsboken till några bilder i .docx-filen. Om False konverteras arbetsboken till några tabeller i .docx-filen. |

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
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


Om AllColumnsInOnePagePerSheet är true, kommer allt kolumninnehåll i ett blad att skrivas ut till endast en sida i resultatet. Bredden på papperstorleken i pagesetup kommer att ignoreras, och de andra inställningarna i pagesetup kommer fortfarande att ha effekt.

**Returns:**
boolean
### getAsFlatOpc() {#getAsFlatOpc--}
```
public boolean getAsFlatOpc()
```


Anger om sparande som en flat opc-fil som kan genereras av Open XML SDK

**Returns:**
boolean
### getAsNormalView() {#getAsNormalView--}
```
public boolean getAsNormalView()
```


Exporterar Excel-fil till docx-fil i normal vy. Om denna egenskap är true kommer ett område att skrivas ut, och ingen skalning kommer att tillämpas. Standardvärdet är false.

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Mappen för temporära filer som kan användas som datacache.

**Remarks**

Om mappen inte har specificerats är standardvärdet för den [CellsHelper.getCacheFolder()](../../com.aspose.cells/cellshelper\#getCacheFolder--). Om dess standardvärde är null eller tomt, eller har specificerats som null eller tomt, kommer ingen cachefil att användas när arbetsboken sparas.

**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Om kontroll av begränsningar i Excel-filen när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32K. När du anger ett värde som är längre än 32K trunkeras det.

**Returns:**
boolean
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```
public boolean getCheckFontCompatibility()
```


Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten.

**Remarks**

Standardvärdet är true. Att inaktivera denna egenskap kan ge bättre prestanda. Men när standard- eller angivet teckensnitt för text/tecken inte kan användas för att rendera det, kan oläsliga tecken (såsom block) uppstå i den genererade pdf-filen. I sådana situationer bör användaren behålla denna egenskap som true så att ett alternativt teckensnitt kan sökas och användas för att rendera texten istället;

**Returns:**
boolean
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta till true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken.

**Remarks**

Standard är true.

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
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Hämtar anpassade inställningar under rendering.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Hämtar standardspråk för redigering.

Se [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Det kan visa/rendera olika layouter för textparagraf när olika redigeringsspråk är inställda. Standard är [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är inställd kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode-tecken.

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedXlsxAsChartDataSource() {#getEmbedXlsxAsChartDataSource--}
```
public boolean getEmbedXlsxAsChartDataSource()
```


Anger om en xlsx-fil ska bäddas in som datakälla för diagrammet.

**Remarks**

Standardvärdet är true.

**Returns:**
boolean
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Inställning för rendering av Emf-metafil.

Se [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

EMF-metafiler identifierade som "EMF+ Dual" kan innehålla både EMF+ poster och EMF-poster. Båda typerna av poster kan användas för att rendera bilden, endast EMF+ poster, eller endast EMF-poster. När [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) är inställd kommer EMF+ poster att parsas under rendering till sidan, annars kommer endast EMF-poster att parsas. Standardvärdet är [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Returns:**
int
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Anger om dokumentegenskaper ska krypteras vid sparande som .xls-fil. Standardvärdet är sant.

**Remarks**

Endast för .xls, .xlsx, .xlsb och .xlsm-filer.

**Returns:**
boolean
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Hämtar färg på rutnätslinjer.

**Remarks**

Den kommer att ignorera inställningarna för rutnätslinjens färg i källfilen.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Hämtar typ av rutnätslinje.

Se [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Standard är Dotted-typ.

**Returns:**
int
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Indikerar om du behöver dölja felet vid rendering. Felet kan vara ett fel i form, bild, diagramrendering osv.

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Om OnePagePerSheet är true, kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de andra inställningarna i pagesetup kommer fortfarande att tillämpas.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut.

**Remarks**

Standard är true.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Hämtar antalet sidor som ska sparas.

**Remarks**

Standard är System.Int32.MaxValue vilket betyder att alla sidor kommer att renderas.

**Example**

Följande exempel visar hur man renderar ett sidintervall (3 och 4) i en Microsoft Excel‑fil till PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Hämtar det 0-baserade indexet för den första sidan som ska sparas.

**Remarks**

Standard är 0.

**Example**

Följande exempel visar hur man renderar ett sidintervall (3 och 4) i en Microsoft Excel‑fil till PDF.

```
         //Open an Excel file
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions options = new PdfSaveOptions();
 
         //Print only Page 3 and Page 4 in the output PDF
         //Starting page index (0-based index)
         options.setPageIndex(3);
         //Number of pages to be printed
         options.setPageCount(2);
 
         //Save the PDF file
         wb.save("output.pdf", options);
```

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Styr/indikera framsteg för sid sparningsprocessen.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintingPageType() {#getPrintingPageType--}
```
public int getPrintingPageType()
```


Anger vilka sidor som inte kommer att skrivas ut.

Se [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Om innehållet i bladet är glest, kommer vissa sidor att vara helt tomma i den genererade pdf‑filen. Om du inte vill ha dessa tomma sidor kan du använda detta alternativ för att utelämna dem.

**Example**

Följande kod utelämnar tomma sidor eller sidor som endast innehåller stilinformation som cellbakgrund, kanter.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //ignore blank pages
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_BLANK);
 
         wb.save("output_ignore_blank_page.pdf", pdfSaveOptions);
 
 
         //ignore blank pages and pages which only contains some style content like cell background
         pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_STYLE);
 
         wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
```

**Returns:**
int
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Anger om den senaste diagramdata ska cachas.

**Returns:**
boolean
### getRenderingBehavior() {#getRenderingBehavior--}
```
public int getRenderingBehavior()
```


Hämtar de Excel-specifika renderingsbeteendena som ska tillämpas.

Se [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

Standardvärdet är [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL).

**Returns:**
int
### getSaveAsEditableShapes() {#getSaveAsEditableShapes--}
```
public boolean getSaveAsEditableShapes()
```


Spara alla ritobjekt som redigerbara former i Word-filen, så att du kan redigera dem i Word.

**Remarks**

Endast för diagram.

**Returns:**
boolean
### getSaveAsEditableShaps() {#getSaveAsEditableShaps--}
```
public boolean getSaveAsEditableShaps()
```


Spara alla ritobjekt som redigerbara former i Word-filen. Så kan du redigera dem i Word.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd i stället [getSaveAsEditableShapes()](../../com.aspose.cells/docxsaveoptions\#getSaveAsEditableShapes--) egenskap. Denna egenskap kommer att tas bort 6 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### getSaveElementType() {#getSaveElementType--}
```
public int getSaveElementType()
```


Anger vilka element som ska sparas.

Se [SaveElementType](../../com.aspose.cells/saveelementtype).

**Returns:**
int
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

**Example**

Följande kod renderar endast det aktiva bladet till pdf.

```
         Workbook workbook = new Workbook("Book1.xlsx");
 
         int activeSheetIndex = workbook.getWorksheets().getActiveSheetIndex();
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
         //set active sheet index to sheet set.
         pdfSaveOptions.setSheetSet(new SheetSet(new int[] { activeSheetIndex }));
         workbook.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Hämtar visningstyp för text när textbredden är större än cellbredden.

Se [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
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
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt.

**Remarks**

Standard är false. Vi kommer först att försöka med standardfonten för Workbook och PdfSaveOption/system för cellfont.

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




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


Om AllColumnsInOnePagePerSheet är true, kommer allt kolumninnehåll i ett blad att skrivas ut till endast en sida i resultatet. Bredden på papperstorleken i pagesetup kommer att ignoreras, och de andra inställningarna i pagesetup kommer fortfarande att ha effekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAsFlatOpc(boolean value) {#setAsFlatOpc-boolean-}
```
public void setAsFlatOpc(boolean value)
```


Anger om sparande som en flat opc-fil som kan genereras av Open XML SDK

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAsNormalView(boolean value) {#setAsNormalView-boolean-}
```
public void setAsNormalView(boolean value)
```


Exporterar Excel-fil till docx-fil i normal vy. Om denna egenskap är true kommer ett område att skrivas ut, och ingen skalning kommer att tillämpas. Standardvärdet är false.

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

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Om kontroll av begränsningar i Excel-filen när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32K. När du anger ett värde som är längre än 32K trunkeras det.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCheckFontCompatibility(boolean value) {#setCheckFontCompatibility-boolean-}
```
public void setCheckFontCompatibility(boolean value)
```


Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten.

**Remarks**

Standardvärdet är true. Att inaktivera denna egenskap kan ge bättre prestanda. Men när standard- eller angivet teckensnitt för text/tecken inte kan användas för att rendera det, kan oläsliga tecken (såsom block) uppstå i den genererade pdf-filen. I sådana situationer bör användaren behålla denna egenskap som true så att ett alternativt teckensnitt kan sökas och användas för att rendera texten istället;

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in detta till true för att försöka använda arbetsbokens standardteckensnitt för att först visa dessa tecken.

**Remarks**

Standard är true.

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

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Ställer in anpassade inställningar under rendering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Ställer in standardspråk för redigering.

Se [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Det kan visa/rendera olika layouter för textparagraf när olika redigeringsspråk är inställda. Standard är [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf, bild. Ställ in DefaultFont, till exempel MingLiu eller MS Gothic, för att visa dessa tecken. Om denna egenskap inte är inställd kommer Aspose.Cells att använda systemets standardteckensnitt för att visa dessa Unicode-tecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedXlsxAsChartDataSource(boolean value) {#setEmbedXlsxAsChartDataSource-boolean-}
```
public void setEmbedXlsxAsChartDataSource(boolean value)
```


Anger om en xlsx-fil ska bäddas in som datakälla för diagrammet.

**Remarks**

Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Inställning för rendering av Emf-metafil.

Se [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

EMF-metafiler identifierade som "EMF+ Dual" kan innehålla både EMF+ poster och EMF-poster. Båda typerna av poster kan användas för att rendera bilden, endast EMF+ poster, eller endast EMF-poster. När [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) är inställd kommer EMF+ poster att parsas under rendering till sidan, annars kommer endast EMF-poster att parsas. Standardvärdet är [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt.

**Remarks**

Standard är false. Vi kommer först att försöka med standardfonten för Workbook och PdfSaveOption/system för cellfont.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Ställer in färg för rutnätslinjer.

**Remarks**

Den kommer att ignorera inställningarna för rutnätslinjens färg i källfilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Ställer in typ för rutnätslinjer.

Se [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Standard är Dotted-typ.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Indikerar om du behöver dölja felet vid rendering. Felet kan vara ett fel i form, bild, diagramrendering osv.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Om OnePagePerSheet är true, kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. Pappersstorleken i pagesetup blir ogiltig, men de andra inställningarna i pagesetup kommer fortfarande att tillämpas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut.

**Remarks**

Standard är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Ställer in antalet sidor som ska sparas.

**Remarks**

Standard är System.Int32.MaxValue vilket betyder att alla sidor kommer att renderas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Ställer in det 0-baserade indexet för den första sidan som ska sparas.

**Remarks**

Standard är 0.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Styr/indikera framsteg för sid sparningsprocessen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintingPageType(int value) {#setPrintingPageType-int-}
```
public void setPrintingPageType(int value)
```


Anger vilka sidor som inte kommer att skrivas ut.

Se [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Remarks**

Om innehållet i bladet är glest, kommer vissa sidor att vara helt tomma i den genererade pdf‑filen. Om du inte vill ha dessa tomma sidor kan du använda detta alternativ för att utelämna dem.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Anger om den senaste diagramdata ska cachas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRenderingBehavior(int value) {#setRenderingBehavior-int-}
```
public void setRenderingBehavior(int value)
```


Ställer in de Excel-specifika renderingsbeteendena som ska tillämpas.

Se [ExcelRenderingBehavior](../../com.aspose.cells/excelrenderingbehavior).

**Remarks**

Standardvärdet är [ExcelRenderingBehavior.ALL](../../com.aspose.cells/excelrenderingbehavior\#ALL).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSaveAsEditableShapes(boolean value) {#setSaveAsEditableShapes-boolean-}
```
public void setSaveAsEditableShapes(boolean value)
```


Spara alla ritobjekt som redigerbara former i Word-filen, så att du kan redigera dem i Word.

**Remarks**

Endast för diagram.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSaveAsEditableShaps(boolean value) {#setSaveAsEditableShaps-boolean-}
```
public void setSaveAsEditableShaps(boolean value)
```


Spara alla ritobjekt som redigerbara former i Word-filen. Så kan du redigera dem i Word.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd i stället [getSaveAsEditableShapes()](../../com.aspose.cells/docxsaveoptions\#getSaveAsEditableShapes--) egenskap. Denna egenskap kommer att tas bort 6 månader senare från och med maj 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSaveElementType(int value) {#setSaveElementType-int-}
```
public void setSaveElementType(int value)
```


Anger vilka element som ska sparas.

Se [SaveElementType](../../com.aspose.cells/saveelementtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Ställer in de blad som ska renderas. Standard är alla synliga blad i arbetsboken: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

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

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Ställer in visningstyp för text när textbredden är större än cellbredden.

Se [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

