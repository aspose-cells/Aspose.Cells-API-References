---
title: "WorkbookSettings"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla inställningar för arbetsboken."
type: docs
url: /sv/java/com.aspose.cells/workbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookSettings
```

Representerar alla inställningar för arbetsboken.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorkbookSettings settings = workbook.getSettings();
 
         //do your business
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [dispose()](#dispose--) | Frigör resurser. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Hämtar filens författare. |
| [getAutoCompressPictures()](#getAutoCompressPictures--) | Anger ett booleskt värde som visar att programmet automatiskt komprimerade bilder i arbetsboken. |
| [getAutoRecover()](#getAutoRecover--) | Anger om filen är markerad för automatisk återställning. |
| [getBuildVersion()](#getBuildVersion--) | Anger den inkrementella offentliga releasen av programmet. |
| [getCheckCompatibility()](#getCheckCompatibility--) | Anger om kompatibilitet med tidigare versioner ska kontrolleras när arbetsboken sparas. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Anger om anpassat talformat ska kontrolleras när Style.Custom ställs in. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getClass()](#getClass--) |  |
| [getCompliance()](#getCompliance--) | Anger OOXML-versionen för utdokumentet. |
| [getCrashSave()](#getCrashSave--) | Anger om programmet senast sparade arbetsboksfilen efter en krasch. |
| [getDataExtractLoad()](#getDataExtractLoad--) | Anger om programmet senast öppnade arbetsboken för dataräddning. |
| [getDate1904()](#getDate1904--) | Hämtar ett värde som visar om arbetsboken använder 1904-datersystemet. |
| [getDefaultImageResolution()](#getDefaultImageResolution--) | Hämtar standardupplösning för bilden. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Hämtar inställningarna för standardvärden för stilrelaterade egenskaper för denna arbetsbok. |
| [getDiscardImageEditData()](#getDiscardImageEditData--) | Anger om redigeringsbilddata ska kasseras. |
| [getDisplayDrawingObjects()](#getDisplayDrawingObjects--) | Anger om och hur objekt ska visas i arbetsboken. |
| [getEnableMacros()](#getEnableMacros--) | Aktivera makron; |
| [getFirstVisibleTab()](#getFirstVisibleTab--) | Hämtar den första synliga arbetsbladstabb. |
| [getFormulaSettings()](#getFormulaSettings--) | Hämtar inställningarna för formelrelaterade funktioner. |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | Hämtar globaliseringsinställningarna. |
| [getHidePivotFieldList()](#getHidePivotFieldList--) | Hämtar om fältlistan för pivottabellen ska döljas. |
| [getLanguageCode()](#getLanguageCode--) | Hämtar användargränssnittsspråket för arbetsboksversionen baserat på landskoden som har sparat filen. |
| [getLocale()](#getLocale--) | Hämtar den lokala inställning som används av denna arbetsbok. |
| [getMaxColumn()](#getMaxColumn--) | Hämtar det maximala kolumnindexet, nollbaserat. |
| [getMaxRow()](#getMaxRow--) | Hämtar det maximala radindexet, nollbaserat. |
| [getMaxRowsOfSharedFormula()](#getMaxRowsOfSharedFormula--) | Hämtar det maximala radnumret för delad formel. |
| [getMaxUniqueItemsPerField()](#getMaxUniqueItemsPerField--) | Hämtar begränsningen av unika objekt per fält |
| [getMemorySetting()](#getMemorySetting--) | Hämtar minnesanvändningsalternativen. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Hämtar decimalavgränsaren för formatering/parsning av numeriska värden. |
| [getNumberGroupSeparator()](#getNumberGroupSeparator--) | Hämtar tecknet som separerar grupper av siffror till vänster om decimalen i numeriska värden. |
| [getPaperSize()](#getPaperSize--) | Hämtar standardpappersstorlek för utskrift. |
| [getPassword()](#getPassword--) | Representerar Workbook-filens krypteringslösenord. |
| [getPropertiesFollowChartPoint()](#getPropertiesFollowChartPoint--) | Anger om datapoint properties and datalabels i alla diagram i denna workbook följer deras referens. |
| [getProtectionType()](#getProtectionType--) | Hämtar skyddstypen för workbook. |
| [getQuotePrefixToStyle()](#getQuotePrefixToStyle--) | Anger om inställning av egenskapen [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) när en strängvärde (som börjar med enkelfnutt) skrivs in i cellen |
| [getRegion()](#getRegion--) | Hämtar de regionala inställningarna för workbook. |
| [getRemovePersonalInformation()](#getRemovePersonalInformation--) | Sant om personlig information kan tas bort från den angivna workbook. |
| [getRepairLoad()](#getRepairLoad--) | Anger om programmet senast öppnade workbook i säkert eller reparationsläge. |
| [getResourceProvider()](#getResourceProvider--) | Hämtar strömleverantören för extern resurs, till exempel inläsning av bilddata för bild av typen "LinkToFile". |
| [getShapeDisplayType()](#getShapeDisplayType--) | Hämtar hur programmet visar former i denna workbook |
| [getShared()](#getShared--) | Hämtar ett värde som indikerar om Workbook är delad. |
| [getSheetTabBarWidth()](#getSheetTabBarWidth--) | Bredd på arbetsbladsflikfältet (i 1/1000 av fönsterbredden). |
| [getShowTabs()](#getShowTabs--) | Hämtar ett värde om Workbook-flikarna visas. |
| [getSignificantDigits()](#getSignificantDigits--) | Hämtar antalet signifikanta siffror. |
| [getSignificantDigitsType()](#getSignificantDigitsType--) | Hämtar typen av signifikanta siffror för utskrift av numeriska värden i denna workbook. |
| [getSmartTagOptions()](#getSmartTagOptions--) | Hämtar alternativen för smart tag. |
| [getStreamProvider()](#getStreamProvider--) | Hämtar strömleverantören för extern resurs. |
| [getThemeFont(int type)](#getThemeFont-int-) | Hämtar standardtema typsnittsnamn. |
| [getUpdateAdjacentCellsBorder()](#getUpdateAdjacentCellsBorder--) | Anger om kantlinjen för intilliggande celler ska uppdateras. |
| [getUpdateLinksType()](#getUpdateLinksType--) | Hämtar hur externa länkar uppdateras när workbook öppnas. |
| [getWarningCallback()](#getWarningCallback--) | Hämtar varningsåteranrop. |
| [getWindowHeight()](#getWindowHeight--) | Fönstrets höjd, i enheten punkt. |
| [getWindowHeightCM()](#getWindowHeightCM--) | Fönstrets höjd, i enheten centimeter. |
| [getWindowHeightInch()](#getWindowHeightInch--) | Fönstrets höjd, i enheten tum. |
| [getWindowLeft()](#getWindowLeft--) | Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret, i enheten punkt. |
| [getWindowLeftCM()](#getWindowLeftCM--) | Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. |
| [getWindowLeftInch()](#getWindowLeftInch--) | Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. |
| [getWindowTop()](#getWindowTop--) | Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet punkt. |
| [getWindowTopCM()](#getWindowTopCM--) | Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet centimeter. |
| [getWindowTopInch()](#getWindowTopInch--) | Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet tum. |
| [getWindowWidth()](#getWindowWidth--) | Bredden på fönstret, i enhet punkt. |
| [getWindowWidthCM()](#getWindowWidthCM--) | Bredden på fönstret, i enhet centimeter. |
| [getWindowWidthInch()](#getWindowWidthInch--) | Bredden på fönstret, i enhet tum. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Anger om den ska vara kompatibel med WPS. |
| [getWriteProtection()](#getWriteProtection--) | Tillhandahåller åtkomst till arbetsbokens skrivskyddsalternativ. |
| [hashCode()](#hashCode--) |  |
| [isDefaultEncrypted()](#isDefaultEncrypted--) | Anger om arbetsboken ska krypteras med standardlösenord om struktur och fönster i arbetsboken är låsta. |
| [isEncrypted()](#isEncrypted--) | Hämtar ett värde som anger om ett lösenord krävs för att öppna denna arbetsbok. |
| [isHScrollBarVisible()](#isHScrollBarVisible--) | Hämtar ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en horisontell rullningslist. |
| [isHidden()](#isHidden--) | Anger om denna arbetsbok är dold. |
| [isMinimized()](#isMinimized--) | Representerar om det genererade kalkylbladet kommer att öppnas minimerat. |
| [isProtected()](#isProtected--) | Hämtar ett värde som anger om strukturen eller fönstret i arbetsboken är skyddat. |
| [isVScrollBarVisible()](#isVScrollBarVisible--) | Hämtar ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en vertikal rullningslist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Ställer in filens författare. |
| [setAutoCompressPictures(boolean value)](#setAutoCompressPictures-boolean-) | Anger ett booleskt värde som visar att programmet automatiskt komprimerade bilder i arbetsboken. |
| [setAutoRecover(boolean value)](#setAutoRecover-boolean-) | Anger om filen är markerad för automatisk återställning. |
| [setBuildVersion(String value)](#setBuildVersion-java.lang.String-) | Anger den inkrementella offentliga releasen av programmet. |
| [setCheckCompatibility(boolean value)](#setCheckCompatibility-boolean-) | Anger om kompatibilitet med tidigare versioner ska kontrolleras när arbetsboken sparas. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Anger om anpassat talformat ska kontrolleras när Style.Custom ställs in. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setCompliance(int value)](#setCompliance-int-) | Anger OOXML-versionen för utdokumentet. |
| [setCrashSave(boolean value)](#setCrashSave-boolean-) | Anger om programmet senast sparade arbetsboksfilen efter en krasch. |
| [setDataExtractLoad(boolean value)](#setDataExtractLoad-boolean-) | Anger om programmet senast öppnade arbetsboken för dataräddning. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Ställer in ett värde som representerar om arbetsboken använder 1904-datumsystemet. |
| [setDefaultEncrypted(boolean value)](#setDefaultEncrypted-boolean-) | Anger om arbetsboken ska krypteras med standardlösenord om struktur och fönster i arbetsboken är låsta. |
| [setDefaultImageResolution(int value)](#setDefaultImageResolution-int-) | Ställer in standardupplösning för bilden. |
| [setDiscardImageEditData(boolean value)](#setDiscardImageEditData-boolean-) | Anger om redigeringsbilddata ska kasseras. |
| [setDisplayDrawingObjects(int value)](#setDisplayDrawingObjects-int-) | Anger om och hur objekt ska visas i arbetsboken. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Aktivera makron; |
| [setFirstVisibleTab(int value)](#setFirstVisibleTab-int-) | Ställer in den första synliga arbetsbladfliken. |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-) | Ställer in globaliseringsinställningarna. |
| [setHScrollBarVisible(boolean value)](#setHScrollBarVisible-boolean-) | Ställer in ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en horisontell rullningslist. |
| [setHidden(boolean value)](#setHidden-boolean-) | Anger om denna arbetsbok är dold. |
| [setHidePivotFieldList(boolean value)](#setHidePivotFieldList-boolean-) | Ställer in om fältlistan för pivottabellen ska döljas. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Ställer in användargränssnittets språk för Workbook-versionen baserat på CountryCode som har sparat filen. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Ställer in den lokala inställning som används av denna arbetsbok. |
| [setMaxRowsOfSharedFormula(int value)](#setMaxRowsOfSharedFormula-int-) | Ställer in maximalt radnummer för delad formel. |
| [setMaxUniqueItemsPerField(int value)](#setMaxUniqueItemsPerField-int-) | Ställer in begränsningen för unika objekt per fält. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Ställer in minnesanvändningsalternativen. |
| [setMinimized(boolean value)](#setMinimized-boolean-) | Representerar om det genererade kalkylbladet kommer att öppnas minimerat. |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Ställer in decimalavgränsaren för formatering/avläsning av numeriska värden. |
| [setNumberGroupSeparator(char value)](#setNumberGroupSeparator-char-) | Ställer in tecknet som separerar grupper av siffror till vänster om decimalen i numeriska värden. |
| [setPageOrientationType(int pageOrientationType)](#setPageOrientationType-int-) | Ställ in typ av utskriftsorientering för hela arbetsboken. |
| [setPaperSize(int value)](#setPaperSize-int-) | Ställer in standardpappersstorlek för utskrift. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Representerar Workbook-filens krypteringslösenord. |
| [setPropertiesFollowChartPoint(boolean value)](#setPropertiesFollowChartPoint-boolean-) | Anger om datapoint properties and datalabels i alla diagram i denna workbook följer deras referens. |
| [setQuotePrefixToStyle(boolean value)](#setQuotePrefixToStyle-boolean-) | Anger om inställning av egenskapen [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) när en strängvärde (som börjar med enkelfnutt) skrivs in i cellen |
| [setRegion(int value)](#setRegion-int-) | Ställer in de regionala inställningarna för arbetsboken. |
| [setRemovePersonalInformation(boolean value)](#setRemovePersonalInformation-boolean-) | Sant om personlig information kan tas bort från den angivna workbook. |
| [setRepairLoad(boolean value)](#setRepairLoad-boolean-) | Anger om programmet senast öppnade workbook i säkert eller reparationsläge. |
| [setResourceProvider(IStreamProvider value)](#setResourceProvider-com.aspose.cells.IStreamProvider-) | Ställer in strömtjänsten för extern resurs, till exempel inläsning av bilddata för bild av typen "LinkToFile". |
| [setShapeDisplayType(int value)](#setShapeDisplayType-int-) | Ställer in hur programmet visar former i den här arbetsboken |
| [setShared(boolean value)](#setShared-boolean-) | Ställer in ett värde som indikerar om arbetsboken är delad. |
| [setSheetTabBarWidth(int value)](#setSheetTabBarWidth-int-) | Bredd på arbetsbladsflikfältet (i 1/1000 av fönsterbredden). |
| [setShowTabs(boolean value)](#setShowTabs-boolean-) | Ställer in ett värde för om arbetsbokflikarna visas. |
| [setSignificantDigits(int value)](#setSignificantDigits-int-) | Ställer in antalet signifikanta siffror. |
| [setSignificantDigitsType(int value)](#setSignificantDigitsType-int-) | Ställer in typen av signifikanta siffror för utskrift av numeriska värden i den här arbetsboken. |
| [setStreamProvider(IStreamProvider value)](#setStreamProvider-com.aspose.cells.IStreamProvider-) | Ställer in strömtjänsten för extern resurs. |
| [setUpdateAdjacentCellsBorder(boolean value)](#setUpdateAdjacentCellsBorder-boolean-) | Anger om kantlinjen för intilliggande celler ska uppdateras. |
| [setUpdateLinksType(int value)](#setUpdateLinksType-int-) | Ställer in hur externa länkar uppdateras när arbetsboken öppnas. |
| [setVScrollBarVisible(boolean value)](#setVScrollBarVisible-boolean-) | Ställer in ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en vertikal rullningslist. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Ställer in varningsåteranrop. |
| [setWindowHeight(double value)](#setWindowHeight-double-) | Fönstrets höjd, i enheten punkt. |
| [setWindowHeightCM(double value)](#setWindowHeightCM-double-) | Fönstrets höjd, i enheten centimeter. |
| [setWindowHeightInch(double value)](#setWindowHeightInch-double-) | Fönstrets höjd, i enheten tum. |
| [setWindowLeft(double value)](#setWindowLeft-double-) | Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret, i enheten punkt. |
| [setWindowLeftCM(double value)](#setWindowLeftCM-double-) | Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. |
| [setWindowLeftInch(double value)](#setWindowLeftInch-double-) | Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. |
| [setWindowTop(double value)](#setWindowTop-double-) | Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet punkt. |
| [setWindowTopCM(double value)](#setWindowTopCM-double-) | Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet centimeter. |
| [setWindowTopInch(double value)](#setWindowTopInch-double-) | Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet tum. |
| [setWindowWidth(double value)](#setWindowWidth-double-) | Bredden på fönstret, i enhet punkt. |
| [setWindowWidthCM(double value)](#setWindowWidthCM-double-) | Bredden på fönstret, i enhet centimeter. |
| [setWindowWidthInch(double value)](#setWindowWidthInch-double-) | Bredden på fönstret, i enhet tum. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Anger om den ska vara kompatibel med WPS. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### dispose() {#dispose--}
```
public void dispose()
```


Frigör resurser.

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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Hämtar filens författare.

**Remarks**

Det är inte inställt, kontrollera [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--) först, sedan kontrollera användaren i Environment.

**Returns:**
java.lang.String
### getAutoCompressPictures() {#getAutoCompressPictures--}
```
public boolean getAutoCompressPictures()
```


Anger ett booleskt värde som visar att programmet automatiskt komprimerade bilder i arbetsboken.

**Returns:**
boolean
### getAutoRecover() {#getAutoRecover--}
```
public boolean getAutoRecover()
```


Anger om filen är markerad för automatisk återställning.

**Returns:**
boolean
### getBuildVersion() {#getBuildVersion--}
```
public String getBuildVersion()
```


Anger den inkrementella offentliga releasen av programmet.

**Returns:**
java.lang.String
### getCheckCompatibility() {#getCheckCompatibility--}
```
public boolean getCheckCompatibility()
```


Anger om kompatibilitet med tidigare versioner ska kontrolleras när arbetsboken sparas.

**Remarks**

Standardvärdet är true. Endast för Excel97-2003 xls- eller xlt-filer.

**Returns:**
boolean
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Anger om anpassat talformat ska kontrolleras när Style.Custom ställs in.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde som är längre än 32 K. När du anger ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett Exception om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan skriva ut hela strängvärdet för andra filformat som CSV. Däremot, om du har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```


Anger OOXML-versionen för utdokumentet. Standardvärdet är Ecma376\_2006.

Se [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Endast för .xlsx-filer.

**Returns:**
int
### getCrashSave() {#getCrashSave--}
```
public boolean getCrashSave()
```


Anger om programmet senast sparade arbetsboksfilen efter en krasch.

**Returns:**
boolean
### getDataExtractLoad() {#getDataExtractLoad--}
```
public boolean getDataExtractLoad()
```


Anger om programmet senast öppnade arbetsboken för dataräddning.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Hämtar ett värde som visar om arbetsboken använder 1904-datersystemet.

**Returns:**
boolean
### getDefaultImageResolution() {#getDefaultImageResolution--}
```
public int getDefaultImageResolution()
```


Hämtar standardupplösning för bilden.

**Returns:**
int
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Hämtar inställningarna för standardvärden för stilrelaterade egenskaper för denna arbetsbok.

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getDiscardImageEditData() {#getDiscardImageEditData--}
```
public boolean getDiscardImageEditData()
```


Anger om redigeringsbilddata ska kasseras.

**Returns:**
boolean
### getDisplayDrawingObjects() {#getDisplayDrawingObjects--}
```
public int getDisplayDrawingObjects()
```


Anger om och hur objekt ska visas i arbetsboken.

Se [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Returns:**
int
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Aktivera makron;

**Remarks**

Nu fungerar det bara när ett kalkylblad kopieras till ett annat kalkylblad i en arbetsbok.

**Returns:**
boolean
### getFirstVisibleTab() {#getFirstVisibleTab--}
```
public int getFirstVisibleTab()
```


Hämtar den första synliga arbetsbladstabb.

**Returns:**
int
### getFormulaSettings() {#getFormulaSettings--}
```
public FormulaSettings getFormulaSettings()
```


Hämtar inställningarna för formelrelaterade funktioner.

**Returns:**
[FormulaSettings](../../com.aspose.cells/formulasettings)
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public GlobalizationSettings getGlobalizationSettings()
```


Hämtar globaliseringsinställningarna.

**Returns:**
[GlobalizationSettings](../../com.aspose.cells/globalizationsettings)
### getHidePivotFieldList() {#getHidePivotFieldList--}
```
public boolean getHidePivotFieldList()
```


Hämtar om fältlistan för pivottabellen ska döljas.

**Returns:**
boolean
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Hämtar användargränssnittsspråket för arbetsboksversionen baserat på landskoden som har sparat filen.

Se [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Hämtar den lokala inställning som används av denna arbetsbok.

**Remarks**

Returnerar null om varken Locale eller [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) är inställda.

**Returns:**
java.util.Locale
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


Hämtar det maximala kolumnindexet, nollbaserat.

**Remarks**

Returnerar 255 om filformatet är Excel97-2003;

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


Hämtar det maximala radindexet, nollbaserat.

**Remarks**

Returnerar 65535 om filformatet är Excel97-2003;

**Returns:**
int
### getMaxRowsOfSharedFormula() {#getMaxRowsOfSharedFormula--}
```
public int getMaxRowsOfSharedFormula()
```


Hämtar det maximala radnumret för delad formel.

**Remarks**

Om talet är för stort fungerar autofiltret mycket långsamt i MS Excel 2013.

**Returns:**
int
### getMaxUniqueItemsPerField() {#getMaxUniqueItemsPerField--}
```
public int getMaxUniqueItemsPerField()
```


Hämtar begränsningen av unika objekt per fält

**Remarks**

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Hämtar minnesanvändningsalternativen. Det nya alternativet kommer att användas som standardalternativ för nysskapade arbetsblad men påverkar inte befintliga arbetsblad.

Se [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

För mer information om minnesläget, se [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Hämtar decimalavgränsaren för formatering/parsning av numeriska värden. Standard är decimalavgränsaren för den aktuella regionen.

**Returns:**
char
### getNumberGroupSeparator() {#getNumberGroupSeparator--}
```
public char getNumberGroupSeparator()
```


Hämtar tecknet som separerar grupper av siffror till vänster om decimalen i numeriska värden. Standard är gruppseparatorn för den aktuella regionen.

**Returns:**
char
### getPaperSize() {#getPaperSize--}
```
public int getPaperSize()
```


Hämtar standardpappersstorlek för utskrift.

Se [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Om det inte finns någon inställning för pappersstorlek kommer MS Excel att använda standardinställningen för skrivaren.

**Returns:**
int
### getPassword() {#getPassword--}
```
public String getPassword()
```


Representerar Workbook-filens krypteringslösenord.

**Returns:**
java.lang.String
### getPropertiesFollowChartPoint() {#getPropertiesFollowChartPoint--}
```
public boolean getPropertiesFollowChartPoint()
```


Anger om datapoint properties and datalabels i alla diagram i denna workbook följer deras referens.

**Returns:**
boolean
### getProtectionType() {#getProtectionType--}
```
public int getProtectionType()
```


Hämtar skyddstypen för workbook.

Se [ProtectionType](../../com.aspose.cells/protectiontype).

**Returns:**
int
### getQuotePrefixToStyle() {#getQuotePrefixToStyle--}
```
public boolean getQuotePrefixToStyle()
```


Anger om inställning av egenskapen [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) när en strängvärde (som börjar med enkelfnutt) skrivs in i cellen

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Hämtar de regionala inställningarna för workbook.

Se [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Regionala inställningar som används av Aspose.Cells‑komponenten för en arbetsbok som laddas från en mallfil: i). För en XLS‑fil finns fält definierade för regionala inställningar och MS Excel sparar regionala inställningsdata i filen när XLS‑filen sparas. Så vi använder den sparade regionen i mallfilen för arbetsboken. Om du inte vill använda den region som sparats i XLS‑filen, återställ den till den förväntade (t.ex. CountryCode.Default) efter att ha laddat mallfilen. Dessutom sparar vi det användarspecificerade värdet (med denna metod) i filen när en XLS‑fil sparas. ii). För andra filformat, såsom XLSX, XLSB … osv., finns inget fält definierat för regionala inställningar i filformatsspecifikationen. Så vi använder de regionala inställningarna i applikationens miljö för arbetsboken. Och det användarspecificerade värdet (med denna metod) kan inte behållas för de genererade filerna med dessa filformat. 2. För visningseffekten i MS Excel: De tillämpade regionala inställningarna här kan bara träda i kraft vid körning med Aspose.Cells‑komponenten och inte när den genererade filen visas i MS Excel. Även för den genererade XLS‑filen där de specificerade regionala inställningsdata har sparats, när den visas/redigeras i MS Excel, är den region som MS Excel använder för formatering alltid standard‑regionalinställningarna i den miljö där MS Excel körs, inte den som sparats i filen. Detta är MS Excels beteende och kan inte ändras via kod.

**Returns:**
int
### getRemovePersonalInformation() {#getRemovePersonalInformation--}
```
public boolean getRemovePersonalInformation()
```


Sant om personlig information kan tas bort från den angivna workbook.

**Remarks**

**Returns:**
boolean
### getRepairLoad() {#getRepairLoad--}
```
public boolean getRepairLoad()
```


Anger om programmet senast öppnade workbook i säkert eller reparationsläge.

**Returns:**
boolean
### getResourceProvider() {#getResourceProvider--}
```
public IStreamProvider getResourceProvider()
```


Hämtar strömleverantören för extern resurs, till exempel inläsning av bilddata för bild av typen "LinkToFile".

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getShapeDisplayType() {#getShapeDisplayType--}
```
public int getShapeDisplayType()
```


Hämtar hur programmet visar former i denna workbook

Se [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Returns:**
int
### getShared() {#getShared--}
```
public boolean getShared()
```


Hämtar ett värde som indikerar om Workbook är delad.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getSheetTabBarWidth() {#getSheetTabBarWidth--}
```
public int getSheetTabBarWidth()
```


Bredd på arbetsbladsflikfältet (i 1/1000 av fönsterbredden).

**Returns:**
int
### getShowTabs() {#getShowTabs--}
```
public boolean getShowTabs()
```


Hämtar ett värde om Workbook-flikarna visas.

**Remarks**

Standardvärdet är true.

**Example**

Följande kod döljer bladflikarna och knapparna för flikrullning i kalkylbladet.

```
         // Hide the spreadsheet tabs.
         workbook.getSettings().setShowTabs(false);
```

**Returns:**
boolean
### getSignificantDigits() {#getSignificantDigits--}
```
public int getSignificantDigits()
```


Hämtar antalet signifikanta siffror. Standardvärdet är [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Kan bara vara 15 eller 17 nu. OBS: Denna medlem är nu föråldrad. Använd istället [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Denna egenskap kommer att tas bort 12 månader senare, från och med juni 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
int
### getSignificantDigitsType() {#getSignificantDigitsType--}
```
public int getSignificantDigitsType()
```


Hämtar typen av signifikanta siffror för att skriva ut numeriska värden i den här arbetsboken. Standardvärdet är [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Se [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Returns:**
int
### getSmartTagOptions() {#getSmartTagOptions--}
```
public SmartTagOptions getSmartTagOptions()
```


Hämtar alternativen för smart tag.

**Returns:**
[SmartTagOptions](../../com.aspose.cells/smarttagoptions)
### getStreamProvider() {#getStreamProvider--}
```
public IStreamProvider getStreamProvider()
```


Hämtar strömleverantören för extern resurs.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ResourceProvider. Denna egenskap kommer att tas bort 12 månader senare, från och med juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[IStreamProvider](../../com.aspose.cells/istreamprovider)
### getThemeFont(int type) {#getThemeFont-int-}
```
public String getThemeFont(int type)
```


Hämtar standardtema typsnittsnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). Typschemat för teckensnittet. |

**Returns:**
java.lang.String -
### getUpdateAdjacentCellsBorder() {#getUpdateAdjacentCellsBorder--}
```
public boolean getUpdateAdjacentCellsBorder()
```


Anger om kantlinjen för intilliggande celler ska uppdateras.

**Remarks**

The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

**Returns:**
boolean
### getUpdateLinksType() {#getUpdateLinksType--}
```
public int getUpdateLinksType()
```


Hämtar hur externa länkar uppdateras när workbook öppnas.

Se [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Hämtar varningsåteranrop.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWindowHeight() {#getWindowHeight--}
```
public double getWindowHeight()
```


Fönstrets höjd, i enheten punkt.

**Returns:**
double
### getWindowHeightCM() {#getWindowHeightCM--}
```
public double getWindowHeightCM()
```


Fönstrets höjd, i enheten centimeter.

**Returns:**
double
### getWindowHeightInch() {#getWindowHeightInch--}
```
public double getWindowHeightInch()
```


Fönstrets höjd, i enheten tum.

**Returns:**
double
### getWindowLeft() {#getWindowLeft--}
```
public double getWindowLeft()
```


Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret, i enheten punkt.

**Returns:**
double
### getWindowLeftCM() {#getWindowLeftCM--}
```
public double getWindowLeftCM()
```


Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. I enheten centimeter.

**Returns:**
double
### getWindowLeftInch() {#getWindowLeftInch--}
```
public double getWindowLeftInch()
```


Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. I enheten tum.

**Returns:**
double
### getWindowTop() {#getWindowTop--}
```
public double getWindowTop()
```


Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet punkt.

**Returns:**
double
### getWindowTopCM() {#getWindowTopCM--}
```
public double getWindowTopCM()
```


Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet centimeter.

**Returns:**
double
### getWindowTopInch() {#getWindowTopInch--}
```
public double getWindowTopInch()
```


Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet tum.

**Returns:**
double
### getWindowWidth() {#getWindowWidth--}
```
public double getWindowWidth()
```


Bredden på fönstret, i enhet punkt.

**Returns:**
double
### getWindowWidthCM() {#getWindowWidthCM--}
```
public double getWindowWidthCM()
```


Bredden på fönstret, i enhet centimeter.

**Returns:**
double
### getWindowWidthInch() {#getWindowWidthInch--}
```
public double getWindowWidthInch()
```


Bredden på fönstret, i enhet tum.

**Returns:**
double
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Anger om den ska vara kompatibel med WPS.

**Returns:**
boolean
### getWriteProtection() {#getWriteProtection--}
```
public WriteProtection getWriteProtection()
```


Tillhandahåller åtkomst till arbetsbokens skrivskyddsalternativ.

**Returns:**
[WriteProtection](../../com.aspose.cells/writeprotection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDefaultEncrypted() {#isDefaultEncrypted--}
```
public boolean isDefaultEncrypted()
```


Anger om arbetsboken ska krypteras med standardlösenord om struktur och fönster i arbetsboken är låsta.

**Remarks**

Standardvärdet är falskt nu. Det är samma som i MS Excel 2013.

**Returns:**
boolean
### isEncrypted() {#isEncrypted--}
```
public boolean isEncrypted()
```


Hämtar ett värde som anger om ett lösenord krävs för att öppna denna arbetsbok.

**Returns:**
boolean
### isHScrollBarVisible() {#isHScrollBarVisible--}
```
public boolean isHScrollBarVisible()
```


Hämtar ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en horisontell rullningslist.

**Remarks**

Standardvärdet är true.

**Example**

Följande kod gör den horisontella rullningslisten osynlig för kalkylbladet.

```
         // Hide the horizontal scroll bar of the Excel file.
         settings.setHScrollBarVisible(false);
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Anger om denna arbetsbok är dold.

**Returns:**
boolean
### isMinimized() {#isMinimized--}
```
public boolean isMinimized()
```


Representerar om det genererade kalkylbladet kommer att öppnas minimerat.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Hämtar ett värde som anger om strukturen eller fönstret i arbetsboken är skyddat.

**Returns:**
boolean
### isVScrollBarVisible() {#isVScrollBarVisible--}
```
public boolean isVScrollBarVisible()
```


Hämtar ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en vertikal rullningslist.

**Remarks**

Standardvärdet är true.

**Example**

Följande kod gör den vertikala rullningslisten osynlig för kalkylbladet.

```
         	// Hide the vertical scroll bar of the Excel file.
         settings.setVScrollBarVisible(false);
```

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Ställer in filens författare.

**Remarks**

Det är inte inställt, kontrollera [BuiltInDocumentPropertyCollection.getAuthor()](../../com.aspose.cells/builtindocumentpropertycollection\#getAuthor--) först, sedan kontrollera användaren i Environment.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setAutoCompressPictures(boolean value) {#setAutoCompressPictures-boolean-}
```
public void setAutoCompressPictures(boolean value)
```


Anger ett booleskt värde som visar att programmet automatiskt komprimerade bilder i arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoRecover(boolean value) {#setAutoRecover-boolean-}
```
public void setAutoRecover(boolean value)
```


Anger om filen är markerad för automatisk återställning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBuildVersion(String value) {#setBuildVersion-java.lang.String-}
```
public void setBuildVersion(String value)
```


Anger den inkrementella offentliga releasen av programmet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCheckCompatibility(boolean value) {#setCheckCompatibility-boolean-}
```
public void setCheckCompatibility(boolean value)
```


Anger om kompatibilitet med tidigare versioner ska kontrolleras när arbetsboken sparas.

**Remarks**

Standardvärdet är true. Endast för Excel97-2003 xls- eller xlt-filer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Anger om anpassat talformat ska kontrolleras när Style.Custom ställs in.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Om restriktioner för Excel-filen ska kontrolleras när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde som är längre än 32 K. När du anger ett värde längre än 32 K, t.ex. med Cell.PutValue(string), får du ett Exception om den här egenskapen är sann. Om egenskapen är falsk accepterar vi ditt inmatade strängvärde som cellens värde så att du senare kan skriva ut hela strängvärdet för andra filformat som CSV. Däremot, om du har angett ett värde som är ogiltigt för Excel-filformatet bör du inte spara arbetsboken som Excel-filformat senare. Annars kan det uppstå oväntade fel i den genererade Excel-filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


Anger OOXML-versionen för utdokumentet. Standardvärdet är Ecma376\_2006.

Se [OoxmlCompliance](../../com.aspose.cells/ooxmlcompliance).

**Remarks**

Endast för .xlsx-filer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCrashSave(boolean value) {#setCrashSave-boolean-}
```
public void setCrashSave(boolean value)
```


Anger om programmet senast sparade arbetsboksfilen efter en krasch.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDataExtractLoad(boolean value) {#setDataExtractLoad-boolean-}
```
public void setDataExtractLoad(boolean value)
```


Anger om programmet senast öppnade arbetsboken för dataräddning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Ställer in ett värde som representerar om arbetsboken använder 1904-datumsystemet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDefaultEncrypted(boolean value) {#setDefaultEncrypted-boolean-}
```
public void setDefaultEncrypted(boolean value)
```


Anger om arbetsboken ska krypteras med standardlösenord om struktur och fönster i arbetsboken är låsta.

**Remarks**

Standardvärdet är falskt nu. Det är samma som i MS Excel 2013.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDefaultImageResolution(int value) {#setDefaultImageResolution-int-}
```
public void setDefaultImageResolution(int value)
```


Ställer in standardupplösning för bilden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDiscardImageEditData(boolean value) {#setDiscardImageEditData-boolean-}
```
public void setDiscardImageEditData(boolean value)
```


Anger om redigeringsbilddata ska kasseras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDisplayDrawingObjects(int value) {#setDisplayDrawingObjects-int-}
```
public void setDisplayDrawingObjects(int value)
```


Anger om och hur objekt ska visas i arbetsboken.

Se [DisplayDrawingObjects](../../com.aspose.cells/displaydrawingobjects).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Aktivera makron;

**Remarks**

Nu fungerar det bara när ett kalkylblad kopieras till ett annat kalkylblad i en arbetsbok.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFirstVisibleTab(int value) {#setFirstVisibleTab-int-}
```
public void setFirstVisibleTab(int value)
```


Ställer in den första synliga arbetsbladfliken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.cells.GlobalizationSettings-}
```
public void setGlobalizationSettings(GlobalizationSettings value)
```


Ställer in globaliseringsinställningarna.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.cells/globalizationsettings) |  |

### setHScrollBarVisible(boolean value) {#setHScrollBarVisible-boolean-}
```
public void setHScrollBarVisible(boolean value)
```


Ställer in ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en horisontell rullningslist.

**Remarks**

Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Anger om denna arbetsbok är dold.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHidePivotFieldList(boolean value) {#setHidePivotFieldList-boolean-}
```
public void setHidePivotFieldList(boolean value)
```


Ställer in om fältlistan för pivottabellen ska döljas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Ställer in användargränssnittets språk för Workbook-versionen baserat på CountryCode som har sparat filen.

Se [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Ställer in den lokala inställning som används av denna arbetsbok.

**Remarks**

Returnerar null om varken Locale eller [getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) är inställda.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Locale |  |

### setMaxRowsOfSharedFormula(int value) {#setMaxRowsOfSharedFormula-int-}
```
public void setMaxRowsOfSharedFormula(int value)
```


Ställer in maximalt radnummer för delad formel.

**Remarks**

Om talet är för stort fungerar autofiltret mycket långsamt i MS Excel 2013.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMaxUniqueItemsPerField(int value) {#setMaxUniqueItemsPerField-int-}
```
public void setMaxUniqueItemsPerField(int value)
```


Ställer in begränsningen för unika objekt per fält.

**Remarks**

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Ställer in minnesanvändningsalternativen. Det nya alternativet kommer att tas som standardalternativ för nysskapade arbetsblad men påverkar inte befintliga arbetsblad.

Se [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

För mer information om minnesläget, se [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMinimized(boolean value) {#setMinimized-boolean-}
```
public void setMinimized(boolean value)
```


Representerar om det genererade kalkylbladet kommer att öppnas minimerat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Ställer in decimalavgränsaren för formatering/parsing av numeriska värden. Standard är decimalavgränsaren för den aktuella regionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char |  |

### setNumberGroupSeparator(char value) {#setNumberGroupSeparator-char-}
```
public void setNumberGroupSeparator(char value)
```


Ställer in tecknet som separerar grupper av siffror till vänster om decimalen i numeriska värden. Standard är grupperingstecknet för den aktuella regionen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char |  |

### setPageOrientationType(int pageOrientationType) {#setPageOrientationType-int-}
```
public void setPageOrientationType(int pageOrientationType)
```


Ställ in typ av utskriftsorientering för hela arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pageOrientationType | int | [PageOrientationType](../../com.aspose.cells/pageorientationtype). Sidorienteringstypen |

### setPaperSize(int value) {#setPaperSize-int-}
```
public void setPaperSize(int value)
```


Ställer in standardpappersstorlek för utskrift.

Se [PaperSizeType](../../com.aspose.cells/papersizetype).

**Remarks**

Om det inte finns någon inställning för pappersstorlek kommer MS Excel att använda standardinställningen för skrivaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Representerar Workbook-filens krypteringslösenord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPropertiesFollowChartPoint(boolean value) {#setPropertiesFollowChartPoint-boolean-}
```
public void setPropertiesFollowChartPoint(boolean value)
```


Anger om datapoint properties and datalabels i alla diagram i denna workbook följer deras referens.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setQuotePrefixToStyle(boolean value) {#setQuotePrefixToStyle-boolean-}
```
public void setQuotePrefixToStyle(boolean value)
```


Anger om inställning av egenskapen [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) när en strängvärde (som börjar med enkelfnutt) skrivs in i cellen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Ställer in de regionala inställningarna för arbetsboken.

Se [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

1. Regionala inställningar som används av Aspose.Cells‑komponenten för en arbetsbok som laddas från en mallfil: i). För en XLS‑fil finns fält definierade för regionala inställningar och MS Excel sparar regionala inställningsdata i filen när XLS‑filen sparas. Så vi använder den sparade regionen i mallfilen för arbetsboken. Om du inte vill använda den region som sparats i XLS‑filen, återställ den till den förväntade (t.ex. CountryCode.Default) efter att ha laddat mallfilen. Dessutom sparar vi det användarspecificerade värdet (med denna metod) i filen när en XLS‑fil sparas. ii). För andra filformat, såsom XLSX, XLSB … osv., finns inget fält definierat för regionala inställningar i filformatsspecifikationen. Så vi använder de regionala inställningarna i applikationens miljö för arbetsboken. Och det användarspecificerade värdet (med denna metod) kan inte behållas för de genererade filerna med dessa filformat. 2. För visningseffekten i MS Excel: De tillämpade regionala inställningarna här kan bara träda i kraft vid körning med Aspose.Cells‑komponenten och inte när den genererade filen visas i MS Excel. Även för den genererade XLS‑filen där de specificerade regionala inställningsdata har sparats, när den visas/redigeras i MS Excel, är den region som MS Excel använder för formatering alltid standard‑regionalinställningarna i den miljö där MS Excel körs, inte den som sparats i filen. Detta är MS Excels beteende och kan inte ändras via kod.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setRemovePersonalInformation(boolean value) {#setRemovePersonalInformation-boolean-}
```
public void setRemovePersonalInformation(boolean value)
```


Sant om personlig information kan tas bort från den angivna workbook.

**Remarks**

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRepairLoad(boolean value) {#setRepairLoad-boolean-}
```
public void setRepairLoad(boolean value)
```


Anger om programmet senast öppnade workbook i säkert eller reparationsläge.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setResourceProvider(IStreamProvider value) {#setResourceProvider-com.aspose.cells.IStreamProvider-}
```
public void setResourceProvider(IStreamProvider value)
```


Ställer in strömtjänsten för extern resurs, till exempel inläsning av bilddata för bild av typen "LinkToFile".

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setShapeDisplayType(int value) {#setShapeDisplayType-int-}
```
public void setShapeDisplayType(int value)
```


Ställer in hur programmet visar former i den här arbetsboken

Se [ShapeDisplayType](../../com.aspose.cells/shapedisplaytype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShared(boolean value) {#setShared-boolean-}
```
public void setShared(boolean value)
```


Ställer in ett värde som indikerar om arbetsboken är delad.

**Remarks**

Standardvärdet är falskt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSheetTabBarWidth(int value) {#setSheetTabBarWidth-int-}
```
public void setSheetTabBarWidth(int value)
```


Bredd på arbetsbladsflikfältet (i 1/1000 av fönsterbredden).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShowTabs(boolean value) {#setShowTabs-boolean-}
```
public void setShowTabs(boolean value)
```


Ställer in ett värde för om arbetsbokflikarna visas.

**Remarks**

Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSignificantDigits(int value) {#setSignificantDigits-int-}
```
public void setSignificantDigits(int value)
```


Ställer in antalet signifikanta siffror. Standardvärdet är [CellsHelper.getSignificantDigits()](../../com.aspose.cells/cellshelper\#getSignificantDigits--).

**Remarks**

Kan bara vara 15 eller 17 nu. OBS: Denna medlem är nu föråldrad. Använd istället [getSignificantDigitsType()](../../com.aspose.cells/workbooksettings\#getSignificantDigitsType--). Denna egenskap kommer att tas bort 12 månader senare, från och med juni 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSignificantDigitsType(int value) {#setSignificantDigitsType-int-}
```
public void setSignificantDigitsType(int value)
```


Ställer in typen av signifikanta siffror för att skriva ut numeriska värden i den här arbetsboken. Standardvärdet är [CellsHelper.getSignificantDigitsType()](../../com.aspose.cells/cellshelper\#getSignificantDigitsType--).

Se [SignificantDigitsType](../../com.aspose.cells/significantdigitstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setStreamProvider(IStreamProvider value) {#setStreamProvider-com.aspose.cells.IStreamProvider-}
```
public void setStreamProvider(IStreamProvider value)
```


Ställer in strömtjänsten för extern resurs.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen ResourceProvider. Denna egenskap kommer att tas bort 12 månader senare, från och med juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IStreamProvider](../../com.aspose.cells/istreamprovider) |  |

### setUpdateAdjacentCellsBorder(boolean value) {#setUpdateAdjacentCellsBorder-boolean-}
```
public void setUpdateAdjacentCellsBorder(boolean value)
```


Anger om kantlinjen för intilliggande celler ska uppdateras.

**Remarks**

The default value is false. For example: the bottom border of the cell A1 is update, the top border of the cell A2 should be changed too.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setUpdateLinksType(int value) {#setUpdateLinksType-int-}
```
public void setUpdateLinksType(int value)
```


Ställer in hur externa länkar uppdateras när arbetsboken öppnas.

Se [UpdateLinksType](../../com.aspose.cells/updatelinkstype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setVScrollBarVisible(boolean value) {#setVScrollBarVisible-boolean-}
```
public void setVScrollBarVisible(boolean value)
```


Ställer in ett värde som indikerar om det genererade kalkylbladet kommer att innehålla en vertikal rullningslist.

**Remarks**

Standardvärdet är true.

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

### setWindowHeight(double value) {#setWindowHeight-double-}
```
public void setWindowHeight(double value)
```


Fönstrets höjd, i enheten punkt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWindowHeightCM(double value) {#setWindowHeightCM-double-}
```
public void setWindowHeightCM(double value)
```


Fönstrets höjd, i enheten centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWindowHeightInch(double value) {#setWindowHeightInch-double-}
```
public void setWindowHeightInch(double value)
```


Fönstrets höjd, i enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWindowLeft(double value) {#setWindowLeft-double-}
```
public void setWindowLeft(double value)
```


Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret, i enheten punkt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWindowLeftCM(double value) {#setWindowLeftCM-double-}
```
public void setWindowLeftCM(double value)
```


Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. I enheten centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWindowLeftInch(double value) {#setWindowLeftInch-double-}
```
public void setWindowLeftInch(double value)
```


Avståndet från vänstra kanten av klientområdet till vänstra kanten av fönstret. I enheten tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWindowTop(double value) {#setWindowTop-double-}
```
public void setWindowTop(double value)
```


Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet punkt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWindowTopCM(double value) {#setWindowTopCM-double-}
```
public void setWindowTopCM(double value)
```


Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWindowTopInch(double value) {#setWindowTopInch-double-}
```
public void setWindowTopInch(double value)
```


Avståndet från den övre kanten av klientområdet till den övre kanten av fönstret, i enhet tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWindowWidth(double value) {#setWindowWidth-double-}
```
public void setWindowWidth(double value)
```


Bredden på fönstret, i enhet punkt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWindowWidthCM(double value) {#setWindowWidthCM-double-}
```
public void setWindowWidthCM(double value)
```


Bredden på fönstret, i enhet centimeter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWindowWidthInch(double value) {#setWindowWidthInch-double-}
```
public void setWindowWidthInch(double value)
```


Bredden på fönstret, i enhet tum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Anger om den ska vara kompatibel med WPS.

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

