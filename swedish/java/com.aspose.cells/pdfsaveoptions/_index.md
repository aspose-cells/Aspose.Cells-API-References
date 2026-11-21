---
title: "PdfSaveOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att spara pdf‑filen."
type: docs
url: /sv/java/com.aspose.cells/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class PdfSaveOptions extends PaginatedSaveOptions
```

Representerar alternativen för att spara pdf‑filen.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Skapar alternativ för att spara PDF-fil. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [getBookmark()](#getBookmark--) | Hämtar [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)-objektet. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Mappen för temporära filer som kan användas som datacache. |
| [getCalculateFormula()](#getCalculateFormula--) | Indikerar om formler ska beräknas innan PDF-filen sparas. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Gör arbetsboken tom efter att filen har sparats. |
| [getCompliance()](#getCompliance--) | Hämtar PDF-standardens efterlevnadsnivå för utdata-dokument. |
| [getCreateDirectory()](#getCreateDirectory--) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [getCreatedTime()](#getCreatedTime--) | Hämtar tiden för generering av PDF-dokumentet. |
| [getCustomPropertiesExport()](#getCustomPropertiesExport--) | Hämtar ett värde som bestämmer hur [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) exporteras till PDF‑fil. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Hämtar anpassade inställningar under rendering. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Hämtar standardspråk för redigering. |
| [getDefaultFont()](#getDefaultFont--) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [getDisplayDocTitle()](#getDisplayDocTitle--) | Anger om fönstrets titelrad ska visa dokumenttiteln. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [getEmbedAttachments()](#getEmbedAttachments--) | Anger om bilagan för Ole‑objekt ska bäddas in i Excel. |
| [getEmbedStandardWindowsFonts()](#getEmbedStandardWindowsFonts--) | Sant för att bädda in TrueType‑typsnitt. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Inställning för rendering av Emf-metafil. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [getExportDocumentStructure()](#getExportDocumentStructure--) | Anger om dokumentstrukturen ska exporteras. |
| [getFontEncoding()](#getFontEncoding--) | Hämtar inbäddad teckenkodning i PDF. |
| [getGridlineColor()](#getGridlineColor--) | Hämtar färg på rutnätslinjer. |
| [getGridlineType()](#getGridlineType--) | Hämtar typ av rutnätslinje. |
| [getIgnoreError()](#getIgnoreError--) | Anger om du behöver dölja felet under rendering. |
| [getImageType()](#getImageType--) | Representerar bildtypen vid konvertering av diagram och form. |
| [getMergeAreas()](#getMergeAreas--) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [getOptimizationType()](#getOptimizationType--) | Hämtar PDF‑optimeringstyp. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [getPageCount()](#getPageCount--) | Hämtar antalet sidor som ska sparas. |
| [getPageIndex()](#getPageIndex--) | Hämtar det 0-baserade indexet för den första sidan som ska sparas. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Styr/indikera framsteg för sid sparningsprocessen. |
| [getPdfCompression()](#getPdfCompression--) | Anger komprimeringsalgoritmen |
| [getPrintingPageType()](#getPrintingPageType--) | Anger vilka sidor som inte kommer att skrivas ut. |
| [getProducer()](#getProducer--) | Hämtar producenten av det genererade PDF‑dokumentet. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Anger om den senaste diagramdata ska cachas. |
| [getRenderingBehavior()](#getRenderingBehavior--) | Hämtar de Excel-specifika renderingsbeteendena som ska tillämpas. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar filformatet för sparning. |
| [getSecurityOptions()](#getSecurityOptions--) | Ställ in dessa alternativ när säkerhet krävs i xls2pdf‑resultatet. |
| [getSheetSet()](#getSheetSet--) | Hämtar bladen som ska renderas. |
| [getSortExternalNames()](#getSortExternalNames--) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [getSortNames()](#getSortNames--) | Anger om definierade namn ska sorteras innan filen sparas. |
| [getTextCrossType()](#getTextCrossType--) | Hämtar visningstyp för text när textbredden är större än cellbredden. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Anger om inställning för SmartArt ska uppdateras. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [getWarningCallback()](#getWarningCallback--) | Hämtar varningsåteranrop. |
| [getWatermark()](#getWatermark--) | Hämtar vattenstämpeln för utdata. |
| [getZoomBehavior()](#getZoomBehavior--) | Hämtar det initiala visningsläget när det genererade PDF‑dokumentet öppnas. |
| [getZoomFactor()](#getZoomFactor--) | Hämtar zoomprocenten som används när [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) är [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR). |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Om AllColumnsInOnePagePerSheet är true kommer allt kolumninnehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [setBookmark(PdfBookmarkEntry value)](#setBookmark-com.aspose.cells.PdfBookmarkEntry-) | Ställer in [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)-objektet. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Mappen för temporära filer som kan användas som datacache. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indikerar om formler ska beräknas innan PDF-filen sparas. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Anger om teckensnittskompatibilitet ska kontrolleras för varje tecken i texten. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [setClearData(boolean value)](#setClearData-boolean-) | Gör arbetsboken tom efter att filen har sparats. |
| [setCompliance(int value)](#setCompliance-int-) | Ställer in PDF‑standardernas efterlevnadsnivå för utdata‑dokument. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Ställer in tiden för generering av PDF‑dokumentet. |
| [setCustomPropertiesExport(int value)](#setCustomPropertiesExport-int-) | Ställer in ett värde som bestämmer hur [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) exporteras till PDF‑fil. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Ställer in anpassade inställningar under rendering. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Ställer in standardspråk för redigering. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | När tecken i Excel är Unicode och inte har rätt teckensnitt inställt i cellstilen kan de visas som block i pdf‑ eller bildformat. |
| [setDisplayDocTitle(boolean value)](#setDisplayDocTitle-boolean-) | Anger om fönstrets titelrad ska visa dokumenttiteln. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering. |
| [setEmbedAttachments(boolean value)](#setEmbedAttachments-boolean-) | Anger om bilagan för Ole‑objekt ska bäddas in i Excel. |
| [setEmbedStandardWindowsFonts(boolean value)](#setEmbedStandardWindowsFonts-boolean-) | Sant för att bädda in TrueType‑typsnitt. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Inställning för rendering av Emf-metafil. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [setExportDocumentStructure(boolean value)](#setExportDocumentStructure-boolean-) | Anger om dokumentstrukturen ska exporteras. |
| [setFontEncoding(int value)](#setFontEncoding-int-) | Ställer in inbäddad teckenkodning i PDF. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Anger om endast teckensnittet för tecknet ska ersättas när cellens teckensnitt inte är kompatibelt. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Ställer in färg för rutnätslinjer. |
| [setGridlineType(int value)](#setGridlineType-int-) | Ställer in typ för rutnätslinjer. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Anger om du behöver dölja felet under rendering. |
| [setImageResample(int desiredPPI, int jpegQuality)](#setImageResample-int-int-) | Ställer in önskad PPI (pixlar per tum) för omprovade bilder och JPEG‑kvalitet. |
| [setImageType(ImageFormat value)](#setImageType-com.aspose.cells.ImageFormat-) | Representerar bildtypen vid konvertering av diagram och form. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Om OnePagePerSheet är true kommer allt innehåll i ett blad att skrivas ut på endast en sida i resultatet. |
| [setOptimizationType(int value)](#setOptimizationType-int-) | Ställer in PDF‑optimeringstyp. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut. |
| [setPageCount(int value)](#setPageCount-int-) | Ställer in antalet sidor som ska sparas. |
| [setPageIndex(int value)](#setPageIndex-int-) | Ställer in det 0-baserade indexet för den första sidan som ska sparas. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Styr/indikera framsteg för sid sparningsprocessen. |
| [setPdfCompression(int value)](#setPdfCompression-int-) | Anger komprimeringsalgoritmen |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Anger vilka sidor som inte kommer att skrivas ut. |
| [setProducer(String value)](#setProducer-java.lang.String-) | Ställer in producenten av det genererade PDF‑dokumentet. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Anger om den senaste diagramdata ska cachas. |
| [setRenderingBehavior(int value)](#setRenderingBehavior-int-) | Ställer in de Excel-specifika renderingsbeteendena som ska tillämpas. |
| [setSecurityOptions(PdfSecurityOptions value)](#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-) | Ställ in dessa alternativ när säkerhet krävs i xls2pdf‑resultatet. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Ställer in vilka blad som ska renderas. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Anger om definierade namn ska sorteras innan filen sparas. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Ställer in visningstyp för text när textbredden är större än cellbredden. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Anger om inställning för SmartArt ska uppdateras. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Ställer in varningsåteranrop. |
| [setWatermark(RenderingWatermark value)](#setWatermark-com.aspose.cells.RenderingWatermark-) | Ställer in vattenstämpeln för utdata. |
| [setZoomBehavior(int value)](#setZoomBehavior-int-) | Ställer in det initiala visningsläget när det genererade PDF‑dokumentet öppnas. |
| [setZoomFactor(int value)](#setZoomFactor-int-) | Ställer in zoomprocenten som används när [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) är [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR). |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Skapar alternativ för att spara PDF-fil.

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
### getBookmark() {#getBookmark--}
```
public PdfBookmarkEntry getBookmark()
```


Hämtar [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)-objektet.

**Returns:**
[PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)
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


Indikerar om formler ska beräknas innan PDF-filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
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
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Hämtar PDF-standardens efterlevnadsnivå för utdata-dokument.

Se [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

Standard är Pdf17.

**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


Hämtar tiden för generering av PDF-dokumentet.

**Remarks**

Om den inte är inställd, blir den tidpunkten för generering av pdf:en.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCustomPropertiesExport() {#getCustomPropertiesExport--}
```
public int getCustomPropertiesExport()
```


Hämtar ett värde som bestämmer hur [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) exporteras till PDF‑fil. Standardvärdet är None.

Se [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Returns:**
int
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
### getDisplayDocTitle() {#getDisplayDocTitle--}
```
public boolean getDisplayDocTitle()
```


Anger om fönstrets titelrad ska visa dokumenttiteln.

**Remarks**

Om falskt, bör namnlisten istället visa namnet på PDF‑filen. Standardvärdet är false.

**Returns:**
boolean
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedAttachments() {#getEmbedAttachments--}
```
public boolean getEmbedAttachments()
```


Anger om bilagan för Ole‑objekt ska bäddas in i Excel.

**Remarks**

Standardvärdet är false. Värdet måste vara false när PDF/A‑efterlevnad är inställd eller pdf‑kryptering är aktiverad.

**Returns:**
boolean
### getEmbedStandardWindowsFonts() {#getEmbedStandardWindowsFonts--}
```
public boolean getEmbedStandardWindowsFonts()
```


Sant för att bädda in TrueType‑teckensnitt. Påverkar endast ASCII‑tecken 32‑127. Teckensnitt för teckenkoder större än 127 bäddas alltid in. Teckensnitt bäddas alltid in för PDF/A-1a, PDF/A-1b‑standarden. Standard är true.

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
### getExportDocumentStructure() {#getExportDocumentStructure--}
```
public boolean getExportDocumentStructure()
```


Anger om dokumentstrukturen ska exporteras.

**Returns:**
boolean
### getFontEncoding() {#getFontEncoding--}
```
public int getFontEncoding()
```


Hämtar inbäddad teckenkodning i PDF.

Se [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

Standardvärdet är [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)

**Returns:**
int
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
### getImageType() {#getImageType--}
```
public ImageFormat getImageType()
```


Representerar bildtypen vid konvertering av diagram och form.

**Remarks**

OBS: Denna medlem är nu föråldrad. Istället renderas Chart och Shape alltid som vektorelement (t.ex. punkt, linje) för renderingskvalitet. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
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
### getOptimizationType() {#getOptimizationType--}
```
public int getOptimizationType()
```


Hämtar PDF‑optimeringstyp.

Se [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

Standardvärdet är [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)

**Returns:**
int
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
### getPdfCompression() {#getPdfCompression--}
```
public int getPdfCompression()
```


Anger komprimeringsalgoritmen

Se [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Returns:**
int
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
### getProducer() {#getProducer--}
```
public String getProducer()
```


Hämtar producenten av det genererade PDF‑dokumentet.

**Remarks**

Om värdet är null, eller en giltig LICENSE inte är inställd, kommer strängen Aspose.Cells vVERSION att användas.

**Returns:**
java.lang.String
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
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Hämtar filformatet för sparning.

Se [SaveFormat](../../com.aspose.cells/saveformat).

**Returns:**
int
### getSecurityOptions() {#getSecurityOptions--}
```
public PdfSecurityOptions getSecurityOptions()
```


Ställ in dessa alternativ när säkerhet krävs i xls2pdf‑resultatet.

**Example**

Följande kod ställer in utskriftsupplösning i höjd för den genererade pdf‑filen.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Returns:**
[PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions)
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
### getWatermark() {#getWatermark--}
```
public RenderingWatermark getWatermark()
```


Hämtar vattenstämpeln för utdata.

**Example**

Följande kod lägger till vattenstämpel i den genererade pdf‑filen.

```
         //prepare a workbook with 3 pages.
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").putValue("Page1");
         int index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page2");
         index = wb.getWorksheets().add();
         wb.getWorksheets().get(index).getCells().get("A1").putValue("Page3");
         wb.getWorksheets().get(index).getPageSetup().setPaperSize(PaperSizeType.PAPER_A_3);
 
         //create a font for watermark, and specify bold, italic, color
         RenderingFont font = new RenderingFont("Calibri", 68);
         font.setItalic(true);
         font.setBold(true);
         font.setColor(Color.getBlue());
 
         //create a watermark from text and the specified font
         RenderingWatermark watermark = new RenderingWatermark("Watermark", font);
 
         //specify horizontal and vertical alignment
         watermark.setHAlignment(TextAlignmentType.CENTER);
         watermark.setVAlignment(TextAlignmentType.CENTER);
 
         //specify rotation
         watermark.setRotation(30);
 
         //specify opacity
         watermark.setOpacity(0.6f);
 
         //specify the scale to page(e.g. 100, 50) in percent.
         watermark.setScaleToPagePercent(50);
 
         //spcify watermark for rendering to pdf.
         PdfSaveOptions options = new PdfSaveOptions();
         options.setWatermark(watermark);
 
         wb.save("output_watermark.pdf", options);
```

**Returns:**
[RenderingWatermark](../../com.aspose.cells/renderingwatermark)
### getZoomBehavior() {#getZoomBehavior--}
```
public int getZoomBehavior()
```


Hämtar det initiala visningsläget när det genererade PDF‑dokumentet öppnas. Standardvärdet är [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\#NONE).

Se [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Returns:**
int
### getZoomFactor() {#getZoomFactor--}
```
public int getZoomFactor()
```


Hämtar zoomprocenten som används när [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) är [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Remarks**

Denna egenskap ignoreras om inte [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) är [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Returns:**
int
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

### setBookmark(PdfBookmarkEntry value) {#setBookmark-com.aspose.cells.PdfBookmarkEntry-}
```
public void setBookmark(PdfBookmarkEntry value)
```


Ställer in [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)-objektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) |  |

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


Indikerar om formler ska beräknas innan PDF-filen sparas.

**Remarks**

Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Ställer in PDF‑standardernas efterlevnadsnivå för utdata‑dokument.

Se [PdfCompliance](../../com.aspose.cells/pdfcompliance).

**Remarks**

Standard är Pdf17.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


Ställer in tiden för generering av PDF‑dokumentet.

**Remarks**

Om den inte är inställd, blir den tidpunkten för generering av pdf:en.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCustomPropertiesExport(int value) {#setCustomPropertiesExport-int-}
```
public void setCustomPropertiesExport(int value)
```


Ställer in ett värde som bestämmer hur [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) exporteras till PDF‑fil. Standardvärdet är None.

Se [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setDisplayDocTitle(boolean value) {#setDisplayDocTitle-boolean-}
```
public void setDisplayDocTitle(boolean value)
```


Anger om fönstrets titelrad ska visa dokumenttiteln.

**Remarks**

Om falskt, bör namnlisten istället visa namnet på PDF‑filen. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implementerar detta gränssnitt för att få DrawObject och Bound vid rendering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedAttachments(boolean value) {#setEmbedAttachments-boolean-}
```
public void setEmbedAttachments(boolean value)
```


Anger om bilagan för Ole‑objekt ska bäddas in i Excel.

**Remarks**

Standardvärdet är false. Värdet måste vara false när PDF/A‑efterlevnad är inställd eller pdf‑kryptering är aktiverad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEmbedStandardWindowsFonts(boolean value) {#setEmbedStandardWindowsFonts-boolean-}
```
public void setEmbedStandardWindowsFonts(boolean value)
```


Sant för att bädda in TrueType‑teckensnitt. Påverkar endast ASCII‑tecken 32‑127. Teckensnitt för teckenkoder större än 127 bäddas alltid in. Teckensnitt bäddas alltid in för PDF/A-1a, PDF/A-1b‑standarden. Standard är true.

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

### setExportDocumentStructure(boolean value) {#setExportDocumentStructure-boolean-}
```
public void setExportDocumentStructure(boolean value)
```


Anger om dokumentstrukturen ska exporteras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFontEncoding(int value) {#setFontEncoding-int-}
```
public void setFontEncoding(int value)
```


Ställer in inbäddad teckenkodning i PDF.

Se [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).

**Remarks**

Standardvärdet är [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setImageResample(int desiredPPI, int jpegQuality) {#setImageResample-int-int-}
```
public void setImageResample(int desiredPPI, int jpegQuality)
```


Ställer in önskad PPI (pixlar per tum) för omprovning av bilder och JPEG‑kvalitet. Alla bilder konverteras till JPEG med den angivna kvalitetsinställningen, och bilder som är större än den angivna PPI (pixlar per tum) kommer att omprovas.

**Example**

Följande kod anger önskad PPI till 96 och JPEG‑kvalitet till 80 för bilder i den genererade pdf‑filen.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
         //set desired PPI as 96 and jpeg quality as 80.
         pdfSaveOptions.setImageResample(96, 80);
 
         wb.save("output.pdf", pdfSaveOptions);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| desiredPPI | int | Önskade pixlar per tum. 220 hög kvalitet. 150 skärmkvalitet. 96 e‑postkvalitet. |
| jpegQuality | int | 0 - 100% JPEG‑kvalitet. |

### setImageType(ImageFormat value) {#setImageType-com.aspose.cells.ImageFormat-}
```
public void setImageType(ImageFormat value)
```


Representerar bildtypen vid konvertering av diagram och form.

**Remarks**

OBS: Denna medlem är nu föråldrad. Istället renderas Chart och Shape alltid som vektorelement (t.ex. punkt, linje) för renderingskvalitet. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

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

### setOptimizationType(int value) {#setOptimizationType-int-}
```
public void setOptimizationType(int value)
```


Ställer in PDF‑optimeringstyp.

Se [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).

**Remarks**

Standardvärdet är [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setPdfCompression(int value) {#setPdfCompression-int-}
```
public void setPdfCompression(int value)
```


Anger komprimeringsalgoritmen

Se [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

### setProducer(String value) {#setProducer-java.lang.String-}
```
public void setProducer(String value)
```


Ställer in producenten av det genererade PDF‑dokumentet.

**Remarks**

Om värdet är null, eller en giltig LICENSE inte är inställd, kommer strängen Aspose.Cells vVERSION att användas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

### setSecurityOptions(PdfSecurityOptions value) {#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-}
```
public void setSecurityOptions(PdfSecurityOptions value)
```


Ställ in dessa alternativ när säkerhet krävs i xls2pdf‑resultatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions) |  |

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

### setWatermark(RenderingWatermark value) {#setWatermark-com.aspose.cells.RenderingWatermark-}
```
public void setWatermark(RenderingWatermark value)
```


Ställer in vattenstämpeln för utdata.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [RenderingWatermark](../../com.aspose.cells/renderingwatermark) |  |

### setZoomBehavior(int value) {#setZoomBehavior-int-}
```
public void setZoomBehavior(int value)
```


Ställer in det initiala visningsläget när det genererade PDF-dokumentet öppnas. Standardvärdet är [PdfZoomBehavior.NONE](../../com.aspose.cells/pdfzoombehavior\#NONE).

Se [PdfZoomBehavior](../../com.aspose.cells/pdfzoombehavior).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setZoomFactor(int value) {#setZoomFactor-int-}
```
public void setZoomFactor(int value)
```


Ställer in zoomprocenten som används när [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) är [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Remarks**

Denna egenskap ignoreras om inte [getZoomBehavior()](../../com.aspose.cells/pdfsaveoptions\#getZoomBehavior--) är [PdfZoomBehavior.ZOOM\_FACTOR](../../com.aspose.cells/pdfzoombehavior\#ZOOM-FACTOR).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

