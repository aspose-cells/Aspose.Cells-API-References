---
title: "TxtLoadOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att läsa in en textfil."
type: docs
url: /sv/java/com.aspose.cells/txtloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions), [com.aspose.cells.AbstractTextLoadOptions](../../com.aspose.cells/abstracttextloadoptions)
```
public class TxtLoadOptions extends AbstractTextLoadOptions
```

Representerar alternativen för att läsa in en textfil.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [TxtLoadOptions()](#TxtLoadOptions--) | Skapar alternativ för att läsa in textfil. |
| [TxtLoadOptions(int loadFormat)](#TxtLoadOptions-int-) | Skapar alternativ för att läsa in textfil. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Anger om data automatiskt filtreras när filerna laddas. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Hämtar auto-fitter-alternativen |
| [getCheckDataValid()](#getCheckDataValid--) | Kontrollera om data är giltiga i mallfilen. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getClass()](#getClass--) |  |
| [getConvertDateTimeData()](#getConvertDateTimeData--) | Hämtar ett värde som anger om strängen i textfilen konverteras till datumdata. |
| [getConvertNumericData()](#getConvertNumericData--) | Hämtar ett värde som anger om strängen i textfilen konverteras till numerisk data. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Hämtar standardstilinställningarna för att initiera stilar i arbetsboken |
| [getEncoding()](#getEncoding--) | Hämtar standardkodningen. |
| [getExtendToNextSheet()](#getExtendToNextSheet--) | Om data ska utökas till nästa blad när rader eller kolumner i data överskrider gränsen. |
| [getFontConfigs()](#getFontConfigs--) | Hämtar individuella teckensnittskonfigurationer. |
| [getHeaderColumnsCount()](#getHeaderColumnsCount--) | Antalet rubrikkolumner som ska upprepas för utökade blad. |
| [getHeaderRowsCount()](#getHeaderRowsCount--) | Antalet rubrikrader som ska upprepas för utökade blad. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignorera data som inte skrivs ut om filen skrivs ut direkt |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Anger om onödiga former ska ignoreras. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Hämtar avbrottsövervakaren. |
| [getKeepPrecision()](#getKeepPrecision--) | Anger om en strängvärde inte ska parsas om längden är 15. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Om oparsade data ska behållas i minnet för arbetsboken när den laddas från mallfilen. |
| [getLanguageCode()](#getLanguageCode--) | Hämtar användargränssnittsspråket för arbetsboksversionen baserat på landskoden som har sparat filen. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Datahanteraren för att bearbeta celldata när mallfilen läses. |
| [getLoadFilter()](#getLoadFilter--) | Filtret som anger hur data ska laddas. |
| [getLoadFormat()](#getLoadFormat--) | Hämtar laddningsformatet. |
| [getLoadStyleStrategy()](#getLoadStyleStrategy--) | Anger strategin för att tillämpa stil på parsade värden när strängvärdet konverteras till tal eller datum/tid. |
| [getLocale()](#getLocale--) | Hämtar de regionala inställningarna som används för arbetsboken som ska laddas. |
| [getMaxColumnCount()](#getMaxColumnCount--) | Det maximala antalet kolumner som kan importeras för ett blad. |
| [getMaxRowCount()](#getMaxRowCount--) | Det maximala antalet rader som kan importeras för ett blad. |
| [getMemorySetting()](#getMemorySetting--) | Hämtar minnesläget för den laddade arbetsboken. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Anger om formeln ska parsas när filen läses. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Anger om pivottabellens cachade poster ska parsas när filen laddas. |
| [getPassword()](#getPassword--) | Hämtar arbetsbokens lösenord. |
| [getPreferredParsers()](#getPreferredParsers--) | Hämtar föredragna värdeparsers för att läsa in textfil. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras när formler hämtas och sätts. |
| [getRegion()](#getRegion--) | Hämtar de regionala inställningarna som används för arbetsboken som ska laddas. |
| [getSeparator()](#getSeparator--) | Hämtar teckenseparator för textfil. |
| [getSeparatorString()](#getSeparatorString--) | Hämtar ett strängvärde som separator. |
| [getStandardFont()](#getStandardFont--) | Ställer in standardteckensnittets namn |
| [getStandardFontSize()](#getStandardFontSize--) | Ställer in standardteckensnittets storlek. |
| [getTextQualifier()](#getTextQualifier--) | Anger textkvalificeraren för cellvärden. |
| [getTreatConsecutiveDelimitersAsOne()](#getTreatConsecutiveDelimitersAsOne--) | Om på varandra följande avgränsare ska behandlas som en. |
| [getTreatQuotePrefixAsValue()](#getTreatQuotePrefixAsValue--) | Anger om det inledande enkla citattecknet ska tas med som en del av värdet i en cell. |
| [getWarningCallback()](#getWarningCallback--) | Hämtar varningsåteranrop. |
| [hasFormula()](#hasFormula--) | Anger om texten är en formel om den börjar med "=","Ställer in ett värde som anger om strängen i textfilen konverteras till datumdata. |
| [hasTextQualifier()](#hasTextQualifier--) | Om det finns en textkvalificerare för cellvärdet. |
| [hashCode()](#hashCode--) |  |
| [isMultiEncoded()](#isMultiEncoded--) | Sant betyder att filen innehåller flera kodningar. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Anger om data automatiskt filtreras när filerna laddas. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Ställer in auto-fitter-alternativen |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Kontrollera om data är giltiga i mallfilen. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setConvertDateTimeData(boolean value)](#setConvertDateTimeData-boolean-) | Ställer in ett värde som anger om strängen i textfilen konverteras till numerisk data. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Ställer in standardkodningen. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Ställer in StreamProviderImportHtmlFile för att importera objekt. |
| [setExtendToNextSheet(boolean value)](#setExtendToNextSheet-boolean-) | Om data ska utökas till nästa blad när rader eller kolumner i data överskrider gränsen. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Ställer in individuella teckensnittskonfigurationer. |
| [setHasFormula(boolean value)](#setHasFormula-boolean-) | Anger om texten är en formel om den börjar med "=","Ställer in ett värde som anger om strängen i textfilen konverteras till datumdata. |
| [setHasTextQualifier(boolean value)](#setHasTextQualifier-boolean-) | Om det finns en textkvalificerare för cellvärdet. |
| [setHeaderColumnsCount(int value)](#setHeaderColumnsCount-int-) | Antalet rubrikkolumner som ska upprepas för utökade blad. |
| [setHeaderRowsCount(int value)](#setHeaderRowsCount-int-) | Antalet rubrikrader som ska upprepas för utökade blad. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignorera data som inte skrivs ut om filen skrivs ut direkt |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Anger om onödiga former ska ignoreras. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Ställer in avbrottsövervakaren. |
| [setKeepPrecision(boolean value)](#setKeepPrecision-boolean-) | Anger om en strängvärde inte ska parsas om längden är 15. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Om oparsade data ska behållas i minnet för arbetsboken när den laddas från mallfilen. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Ställer in användargränssnittets språk för Workbook-versionen baserat på CountryCode som har sparat filen. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Datahanteraren för att bearbeta celldata när mallfilen läses. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Filtret som anger hur data ska laddas. |
| [setLoadStyleStrategy(int value)](#setLoadStyleStrategy-int-) | Anger strategin för att tillämpa stil på parsade värden när strängvärdet konverteras till tal eller datum/tid. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Ställer in de regionala inställningarna som används för Workbook som ska laddas. |
| [setMaxColumnCount(int value)](#setMaxColumnCount-int-) | Det maximala antalet kolumner som kan importeras för ett blad. |
| [setMaxRowCount(int value)](#setMaxRowCount-int-) | Det maximala antalet rader som kan importeras för ett blad. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Ställer in minnesläget för den laddade arbetsboken. |
| [setMultiEncoded(boolean value)](#setMultiEncoded-boolean-) | Sant betyder att filen innehåller flera kodningar. |
| [setPaperSize(int type)](#setPaperSize-int-) | Ställer in standardpappersstorlek för utskrift från standardskrivarens inställning. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Anger om formeln ska parsas när filen läses. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Anger om pivottabellens cachade poster ska parsas när filen laddas. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Ställer in lösenordet för arbetsboken. |
| [setPreferredParsers(ICustomParser[] value)](#setPreferredParsers-com.aspose.cells.ICustomParser---) | Ställer in föredragna värdeparsers för att läsa in textfil. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras när formler hämtas och sätts. |
| [setRegion(int value)](#setRegion-int-) | Ställer in de regionala inställningarna som används för Workbook som ska laddas. |
| [setSeparator(char value)](#setSeparator-char-) | Ställer in teckenseparator för textfil. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Ställer in ett strängvärde som separator. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Ställer in standardteckensnittets namn |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Ställer in standardteckensnittets storlek. |
| [setTextQualifier(char value)](#setTextQualifier-char-) | Anger textkvalificeraren för cellvärden. |
| [setTreatConsecutiveDelimitersAsOne(boolean value)](#setTreatConsecutiveDelimitersAsOne-boolean-) | Om på varandra följande avgränsare ska behandlas som en. |
| [setTreatQuotePrefixAsValue(boolean value)](#setTreatQuotePrefixAsValue-boolean-) | Anger om det inledande enkla citattecknet ska tas med som en del av värdet i en cell. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Ställer in varningsåteranrop. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtLoadOptions() {#TxtLoadOptions--}
```
public TxtLoadOptions()
```


Skapar alternativ för att läsa in textfil.

**Remarks**

Standardfiltypen för inläsning är CSV.

### TxtLoadOptions(int loadFormat) {#TxtLoadOptions-int-}
```
public TxtLoadOptions(int loadFormat)
```


Skapar alternativ för att läsa in textfil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadFormat | int | [LoadFormat](../../com.aspose.cells/loadformat). Laddningsformatet |

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
### getAutoFilter() {#getAutoFilter--}
```
public boolean getAutoFilter()
```


Anger om data automatiskt filtreras när filerna laddas.

**Remarks**

Ibland, även om autofilter är inställt, döljs inte motsvarande rader i filen. Fungerar nu endast för SpreadSheetML-filen.

**Returns:**
boolean
### getAutoFitterOptions() {#getAutoFitterOptions--}
```
public AutoFitterOptions getAutoFitterOptions()
```


Hämtar auto-fitter-alternativen

**Remarks**

Endast för xlsx-, spreadsheetML-filer nu.

**Returns:**
[AutoFitterOptions](../../com.aspose.cells/autofitteroptions)
### getCheckDataValid() {#getCheckDataValid--}
```
public boolean getCheckDataValid()
```


Kontrollera om data är giltiga i mallfilen.

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
### getConvertDateTimeData() {#getConvertDateTimeData--}
```
public boolean getConvertDateTimeData()
```


Hämtar ett värde som indikerar om strängen i textfilen konverteras till datumdata. Standardvärdet är true.

**Returns:**
boolean
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Hämtar ett värde som indikerar om strängen i textfilen konverteras till numerisk data. Standardvärdet är true.

**Returns:**
boolean
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Hämtar standardstilinställningarna för att initiera stilar i arbetsboken

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Hämtar standardkodningen. Gäller endast för csv-filer.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getExtendToNextSheet() {#getExtendToNextSheet--}
```
public boolean getExtendToNextSheet()
```


Om data ska utökas till nästa blad när rader eller kolumner i data överskrider gränsen. Standard är falskt.

**Remarks**

Om denna egenskap är sann kommer extra data att placeras i nästa blad bakom det aktuella (om det aktuella bladet är det sista, kommer ett nytt blad att läggas till i den aktuella arbetsboken). Om denna egenskap är falsk kommer data som överskrider gränsen att ignoreras.

**Returns:**
boolean
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Hämtar individuella teckensnittskonfigurationer. Fungerar endast för den [Workbook](../../com.aspose.cells/workbook) som använder dessa [LoadOptions](../../com.aspose.cells/loadoptions) för att laddas.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getHeaderColumnsCount() {#getHeaderColumnsCount--}
```
public int getHeaderColumnsCount()
```


Antalet rubrikkolumner som ska upprepas för utökade blad.

**Remarks**

De rubrikkolumner som anges av denna egenskap kommer att dupliceras för de utökade bladen. Denna egenskap gäller endast när [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) är sann.

**Returns:**
int
### getHeaderRowsCount() {#getHeaderRowsCount--}
```
public int getHeaderRowsCount()
```


Antalet rubrikrader som ska upprepas för utökade blad.

**Remarks**

De rubrikrader som anges av denna egenskap kommer att dupliceras för de utökade bladen. Denna egenskap gäller endast när [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) är sann.

**Returns:**
int
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignorera data som inte skrivs ut om filen skrivs ut direkt

**Remarks**

Endast för xlsx-fil.

**Returns:**
boolean
### getIgnoreUselessShapes() {#getIgnoreUselessShapes--}
```
public boolean getIgnoreUselessShapes()
```


Anger om onödiga former ska ignoreras.

**Remarks**

Fungerar endast för xlsx-, xlsb- och xlsm-filer. Det finns många överlappande identiska former som är onödiga i vissa filer, vi kan ignorera dem när vi laddar filer.

**Returns:**
boolean
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Hämtar avbrottsövervakaren.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getKeepPrecision() {#getKeepPrecision--}
```
public boolean getKeepPrecision()
```


Anger om en strängvärde inte ska parsas om längden är 15.

**Returns:**
boolean
### getKeepUnparsedData() {#getKeepUnparsedData--}
```
public boolean getKeepUnparsedData()
```


Om oparsade data ska behållas i minnet för Workbook när den laddas från en mallfil. Standard är true.

**Remarks**

För scenarier där användaren bara behöver läsa vissa innehåll från mallfilen och inte behöver spara arbetsboken igen, kan du sätta denna egenskap till false för att förbättra prestanda, särskilt när den används tillsammans med någon typ av LoadFilter,

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
### getLightCellsDataHandler() {#getLightCellsDataHandler--}
```
public LightCellsDataHandler getLightCellsDataHandler()
```


Datahanteraren för att bearbeta celldata när mallfilen läses.

**Returns:**
[LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler)
### getLoadFilter() {#getLoadFilter--}
```
public LoadFilter getLoadFilter()
```


Filtret som anger hur data ska laddas.

**Returns:**
[LoadFilter](../../com.aspose.cells/loadfilter)
### getLoadFormat() {#getLoadFormat--}
```
public int getLoadFormat()
```


Hämtar laddningsformatet.

Se [LoadFormat](../../com.aspose.cells/loadformat).

**Returns:**
int
### getLoadStyleStrategy() {#getLoadStyleStrategy--}
```
public int getLoadStyleStrategy()
```


Anger strategin för att tillämpa stil på parsade värden när strängvärdet konverteras till tal eller datum/tid.

Se [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Returns:**
int
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Hämtar de regionala inställningarna som används för arbetsboken som ska laddas.

**Remarks**

Denna egenskap har samma effekt som [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) för att ställa in regionala inställningar.

**Returns:**
java.util.Locale
### getMaxColumnCount() {#getMaxColumnCount--}
```
public int getMaxColumnCount()
```


Det maximala antalet kolumner som kan importeras för ett blad.

**Remarks**

Kolumner som överskrider denna gräns kommer att ignoreras eller utökas till nästa blad enligt [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Detta antal inkluderar rubrikkolumnerna ([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)). Det maximala värdet är kolumngränsen för motsvarande filformat, till exempel för xlsx-filer är det 16384. Om denna egenskap inte har angetts eller det angivna värdet inte är positivt, kommer den maximala gränsen också att användas.

**Returns:**
int
### getMaxRowCount() {#getMaxRowCount--}
```
public int getMaxRowCount()
```


Det maximala antalet rader som kan importeras för ett blad.

**Remarks**

Rader som överskrider denna gräns kommer att ignoreras eller utökas till nästa blad enligt [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Detta antal inkluderar rubrikraderna ([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)). Det maximalt tillåtna värdet är radgränsen för motsvarande filformat, till exempel för xlsx-filer är det 1048576. Om denna egenskap inte har angetts eller det angivna värdet inte är positivt, kommer den maximala gränsen också att användas.

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


Hämtar minnesläget för den laddade arbetsboken.

Se [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

För mer information om minnesläget, se [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Returns:**
int
### getParsingFormulaOnOpen() {#getParsingFormulaOnOpen--}
```
public boolean getParsingFormulaOnOpen()
```


Anger om formeln ska parsas när filen läses.

**Remarks**

Gäller endast för Excel Xlsx, Xltx, Xltm och Xlsm-filer eftersom formlerna i filerna lagras som en strängformel.

**Returns:**
boolean
### getParsingPivotCachedRecords() {#getParsingPivotCachedRecords--}
```
public boolean getParsingPivotCachedRecords()
```


Anger om pivot-cachade poster ska parsas vid inläsning av filen. Standardvärdet är false.

**Remarks**

Gäller endast för Excel Xlsx, Xltx, Xltm, Xlsm och xlsb-filer

**Returns:**
boolean
### getPassword() {#getPassword--}
```
public String getPassword()
```


Hämtar arbetsbokens lösenord.

**Returns:**
java.lang.String
### getPreferredParsers() {#getPreferredParsers--}
```
public ICustomParser[] getPreferredParsers()
```


Hämtar föredragna värdeparsers för att läsa in textfil.

**Remarks**

parsers[0] är den parser som används för den första kolumnen i textmallfilen, parsers[1] är den parser som används för den andra kolumnen, ... osv. Den sista (parsers[parsers.length-1]) kommer att användas för alla andra kolumner från parsers.length-1. Om ett objekt är null kommer motsvarande kolumn att parsas av standardparsern i Aspose.Cells.

**Returns:**
com.aspose.cells.ICustomParser[]
### getPreservePaddingSpacesInFormula() {#getPreservePaddingSpacesInFormula--}
```
public boolean getPreservePaddingSpacesInFormula()
```


Anger om de mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.

**Remarks**

Efter att arbetsboken har lästs in från mallfilen med detta alternativ kommer [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) att sättas till samma värde som denna egenskap.

**Returns:**
boolean
### getRegion() {#getRegion--}
```
public int getRegion()
```


Hämtar de regionala inställningarna som används för arbetsboken som ska laddas.

Se [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

De regionala inställningarna kan användas för att initiera vissa funktioner för arbetsboken, såsom teckensnitt, teman osv. För textbaserade filformat, såsom CSV, HTML, …, kommer den regionala inställningen också att användas för att upptäcka talformat och tolka textvärden till numeriska eller datum/tidsvärden för celler. Denna inställning kommer att behållas för den skapade arbetsboken senare, det vill säga [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) i arbetsboken kommer att använda samma region som denna egenskap.

**Returns:**
int
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Hämtar teckenseparator för textfil.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Hämtar ett strängvärde som separator.

**Returns:**
java.lang.String
### getStandardFont() {#getStandardFont--}
```
public String getStandardFont()
```


Ställer in standardteckensnittets namn

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället DefaultStyleSettings. Denna egenskap kommer att tas bort 12 månader senare från och med mars 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.String
### getStandardFontSize() {#getStandardFontSize--}
```
public double getStandardFontSize()
```


Ställer in standardteckensnittets storlek.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället DefaultStyleSettings. Denna egenskap kommer att tas bort 12 månader senare från och med mars 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
double
### getTextQualifier() {#getTextQualifier--}
```
public char getTextQualifier()
```


Anger textkvalificeraren för cellvärden. Standardkvalificerare är '"'.

**Remarks**

När denna egenskap sätts kommer [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) att automatiskt bli sann.

**Returns:**
char
### getTreatConsecutiveDelimitersAsOne() {#getTreatConsecutiveDelimitersAsOne--}
```
public boolean getTreatConsecutiveDelimitersAsOne()
```


Om på varandra följande avgränsare ska behandlas som en.

**Returns:**
boolean
### getTreatQuotePrefixAsValue() {#getTreatQuotePrefixAsValue--}
```
public boolean getTreatQuotePrefixAsValue()
```


Indikerar om det inledande enkla citattecknet ska tas som en del av värdet i en cell. Standard är sant. Om det är falskt kommer det inledande enkla citattecknet att tas bort från motsvarande cells värde och [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) kommer att sättas till sant för cellen.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Hämtar varningsåteranrop.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hasFormula() {#hasFormula--}
```
public boolean hasFormula()
```


Anger om texten är en formel om den börjar med "=","Ställer in ett värde som anger om strängen i textfilen konverteras till datumdata.

**Returns:**
boolean
### hasTextQualifier() {#hasTextQualifier--}
```
public boolean hasTextQualifier()
```


Om det finns en textkvalificerare för cellvärdet. Standard är sant.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isMultiEncoded() {#isMultiEncoded--}
```
public boolean isMultiEncoded()
```


Sant betyder att filen innehåller flera kodningar.

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




### setAutoFilter(boolean value) {#setAutoFilter-boolean-}
```
public void setAutoFilter(boolean value)
```


Anger om data automatiskt filtreras när filerna laddas.

**Remarks**

Ibland, även om autofilter är inställt, döljs inte motsvarande rader i filen. Fungerar nu endast för SpreadSheetML-filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setAutoFitterOptions(AutoFitterOptions value) {#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-}
```
public void setAutoFitterOptions(AutoFitterOptions value)
```


Ställer in auto-fitter-alternativen

**Remarks**

Endast för xlsx-, spreadsheetML-filer nu.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [AutoFitterOptions](../../com.aspose.cells/autofitteroptions) |  |

### setCheckDataValid(boolean value) {#setCheckDataValid-boolean-}
```
public void setCheckDataValid(boolean value)
```


Kontrollera om data är giltiga i mallfilen.

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

### setConvertDateTimeData(boolean value) {#setConvertDateTimeData-boolean-}
```
public void setConvertDateTimeData(boolean value)
```


Ställer in ett värde som indikerar om strängen i textfilen konverteras till datumdata. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Ställer in ett värde som indikerar om strängen i textfilen konverteras till numerisk data. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Ställer in standardkodningen. Gäller endast för csv-filer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setExtendToNextSheet(boolean value) {#setExtendToNextSheet-boolean-}
```
public void setExtendToNextSheet(boolean value)
```


Om data ska utökas till nästa blad när rader eller kolumner i data överskrider gränsen. Standard är falskt.

**Remarks**

Om denna egenskap är sann kommer extra data att placeras i nästa blad bakom det aktuella (om det aktuella bladet är det sista, kommer ett nytt blad att läggas till i den aktuella arbetsboken). Om denna egenskap är falsk kommer data som överskrider gränsen att ignoreras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Ställer in individuella teckensnittskonfigurationer. Fungerar endast för den [Workbook](../../com.aspose.cells/workbook) som använder dessa [LoadOptions](../../com.aspose.cells/loadoptions) för att läsa in.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

### setHasFormula(boolean value) {#setHasFormula-boolean-}
```
public void setHasFormula(boolean value)
```


Anger om texten är en formel om den börjar med "=","Ställer in ett värde som anger om strängen i textfilen konverteras till datumdata.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasTextQualifier(boolean value) {#setHasTextQualifier-boolean-}
```
public void setHasTextQualifier(boolean value)
```


Om det finns en textkvalificerare för cellvärdet. Standard är sant.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHeaderColumnsCount(int value) {#setHeaderColumnsCount-int-}
```
public void setHeaderColumnsCount(int value)
```


Antalet rubrikkolumner som ska upprepas för utökade blad.

**Remarks**

De rubrikkolumner som anges av denna egenskap kommer att dupliceras för de utökade bladen. Denna egenskap gäller endast när [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) är sann.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setHeaderRowsCount(int value) {#setHeaderRowsCount-int-}
```
public void setHeaderRowsCount(int value)
```


Antalet rubrikrader som ska upprepas för utökade blad.

**Remarks**

De rubrikrader som anges av denna egenskap kommer att dupliceras för de utökade bladen. Denna egenskap gäller endast när [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--) är sann.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setIgnoreNotPrinted(boolean value) {#setIgnoreNotPrinted-boolean-}
```
public void setIgnoreNotPrinted(boolean value)
```


Ignorera data som inte skrivs ut om filen skrivs ut direkt

**Remarks**

Endast för xlsx-fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setIgnoreUselessShapes(boolean value) {#setIgnoreUselessShapes-boolean-}
```
public void setIgnoreUselessShapes(boolean value)
```


Anger om onödiga former ska ignoreras.

**Remarks**

Fungerar endast för xlsx-, xlsb- och xlsm-filer. Det finns många överlappande identiska former som är onödiga i vissa filer, vi kan ignorera dem när vi laddar filer.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Ställer in avbrottsövervakaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setKeepPrecision(boolean value) {#setKeepPrecision-boolean-}
```
public void setKeepPrecision(boolean value)
```


Anger om en strängvärde inte ska parsas om längden är 15.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setKeepUnparsedData(boolean value) {#setKeepUnparsedData-boolean-}
```
public void setKeepUnparsedData(boolean value)
```


Om oparsade data ska behållas i minnet för Workbook när den laddas från en mallfil. Standard är true.

**Remarks**

För scenarier där användaren bara behöver läsa vissa innehåll från mallfilen och inte behöver spara arbetsboken igen, kan du sätta denna egenskap till false för att förbättra prestanda, särskilt när den används tillsammans med någon typ av LoadFilter,

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

### setLightCellsDataHandler(LightCellsDataHandler value) {#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-}
```
public void setLightCellsDataHandler(LightCellsDataHandler value)
```


Datahanteraren för att bearbeta celldata när mallfilen läses.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [LightCellsDataHandler](../../com.aspose.cells/lightcellsdatahandler) |  |

### setLoadFilter(LoadFilter value) {#setLoadFilter-com.aspose.cells.LoadFilter-}
```
public void setLoadFilter(LoadFilter value)
```


Filtret som anger hur data ska laddas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [LoadFilter](../../com.aspose.cells/loadfilter) |  |

### setLoadStyleStrategy(int value) {#setLoadStyleStrategy-int-}
```
public void setLoadStyleStrategy(int value)
```


Anger strategin för att tillämpa stil på parsade värden när strängvärdet konverteras till tal eller datum/tid.

Se [TxtLoadStyleStrategy](../../com.aspose.cells/txtloadstylestrategy).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setLocale(Locale value) {#setLocale-java.util.Locale-}
```
public void setLocale(Locale value)
```


Ställer in de regionala inställningarna som används för Workbook som ska laddas.

**Remarks**

Denna egenskap har samma effekt som [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) för att ställa in regionala inställningar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Locale |  |

### setMaxColumnCount(int value) {#setMaxColumnCount-int-}
```
public void setMaxColumnCount(int value)
```


Det maximala antalet kolumner som kan importeras för ett blad.

**Remarks**

Kolumner som överskrider denna gräns kommer att ignoreras eller utökas till nästa blad enligt [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Detta antal inkluderar rubrikkolumnerna ([getHeaderColumnsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderColumnsCount--)). Det maximala värdet är kolumngränsen för motsvarande filformat, till exempel för xlsx-filer är det 16384. Om denna egenskap inte har angetts eller det angivna värdet inte är positivt, kommer den maximala gränsen också att användas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMaxRowCount(int value) {#setMaxRowCount-int-}
```
public void setMaxRowCount(int value)
```


Det maximala antalet rader som kan importeras för ett blad.

**Remarks**

Rader som överskrider denna gräns kommer att ignoreras eller utökas till nästa blad enligt [getExtendToNextSheet()](../../com.aspose.cells/txtloadoptions\#getExtendToNextSheet--). Detta antal inkluderar rubrikraderna ([getHeaderRowsCount()](../../com.aspose.cells/txtloadoptions\#getHeaderRowsCount--)). Det maximalt tillåtna värdet är radgränsen för motsvarande filformat, till exempel för xlsx-filer är det 1048576. Om denna egenskap inte har angetts eller det angivna värdet inte är positivt, kommer den maximala gränsen också att användas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


Ställer in minnesläget för den laddade arbetsboken.

Se [MemorySetting](../../com.aspose.cells/memorysetting).

**Remarks**

För mer information om minnesläget, se [Cells.getMemorySetting()](../../com.aspose.cells/cells\#getMemorySetting--).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setMultiEncoded(boolean value) {#setMultiEncoded-boolean-}
```
public void setMultiEncoded(boolean value)
```


Sant betyder att filen innehåller flera kodningar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPaperSize(int type) {#setPaperSize-int-}
```
public void setPaperSize(int type)
```


Ställer in standardpappersstorlek för utskrift från standardskrivarens inställning.

**Remarks**

Om det inte finns någon inställning för pappersstorlek kommer MS Excel att använda standardinställningen för skrivaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [PaperSizeType](../../com.aspose.cells/papersizetype). Standardpappersstorleken. |

### setParsingFormulaOnOpen(boolean value) {#setParsingFormulaOnOpen-boolean-}
```
public void setParsingFormulaOnOpen(boolean value)
```


Anger om formeln ska parsas när filen läses.

**Remarks**

Gäller endast för Excel Xlsx, Xltx, Xltm och Xlsm-filer eftersom formlerna i filerna lagras som en strängformel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setParsingPivotCachedRecords(boolean value) {#setParsingPivotCachedRecords-boolean-}
```
public void setParsingPivotCachedRecords(boolean value)
```


Anger om pivot-cachade poster ska parsas vid inläsning av filen. Standardvärdet är false.

**Remarks**

Gäller endast för Excel Xlsx, Xltx, Xltm, Xlsm och xlsb-filer

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


Ställer in lösenordet för arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setPreferredParsers(ICustomParser[] value) {#setPreferredParsers-com.aspose.cells.ICustomParser---}
```
public void setPreferredParsers(ICustomParser[] value)
```


Ställer in föredragna värdeparsers för att läsa in textfil.

**Remarks**

parsers[0] är den parser som används för den första kolumnen i textmallfilen, parsers[1] är den parser som används för den andra kolumnen, ... osv. Den sista (parsers[parsers.length-1]) kommer att användas för alla andra kolumner från parsers.length-1. Om ett objekt är null kommer motsvarande kolumn att parsas av standardparsern i Aspose.Cells.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ICustomParser\[\]](../../com.aspose.cells/icustomparser) |  |

### setPreservePaddingSpacesInFormula(boolean value) {#setPreservePaddingSpacesInFormula-boolean-}
```
public void setPreservePaddingSpacesInFormula(boolean value)
```


Anger om de mellanslag och radbrytningar som är utfyllda mellan formeltoken ska bevaras vid hämtning och inställning av formler. Standardvärdet är falskt.

**Remarks**

Efter att arbetsboken har lästs in från mallfilen med detta alternativ kommer [FormulaSettings.getPreservePaddingSpaces()](../../com.aspose.cells/formulasettings\#getPreservePaddingSpaces--) att sättas till samma värde som denna egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRegion(int value) {#setRegion-int-}
```
public void setRegion(int value)
```


Ställer in de regionala inställningarna som används för Workbook som ska laddas.

Se [CountryCode](../../com.aspose.cells/countrycode).

**Remarks**

De regionala inställningarna kan användas för att initiera vissa funktioner för arbetsboken, såsom teckensnitt, teman osv. För textbaserade filformat, såsom CSV, HTML, …, kommer den regionala inställningen också att användas för att upptäcka talformat och tolka textvärden till numeriska eller datum/tidsvärden för celler. Denna inställning kommer att behållas för den skapade arbetsboken senare, det vill säga [WorkbookSettings.getRegion()](../../com.aspose.cells/workbooksettings\#getRegion--) i arbetsboken kommer att använda samma region som denna egenskap.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Ställer in teckenseparator för textfil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Ställer in ett strängvärde som separator.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setStandardFont(String value) {#setStandardFont-java.lang.String-}
```
public void setStandardFont(String value)
```


Ställer in standardteckensnittets namn

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället DefaultStyleSettings. Denna egenskap kommer att tas bort 12 månader senare från och med mars 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setStandardFontSize(double value) {#setStandardFontSize-double-}
```
public void setStandardFontSize(double value)
```


Ställer in standardteckensnittets storlek.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället DefaultStyleSettings. Denna egenskap kommer att tas bort 12 månader senare från och med mars 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setTextQualifier(char value) {#setTextQualifier-char-}
```
public void setTextQualifier(char value)
```


Anger textkvalificeraren för cellvärden. Standardkvalificerare är '"'.

**Remarks**

När denna egenskap sätts kommer [hasTextQualifier()](../../com.aspose.cells/txtloadoptions\#hasTextQualifier--) att automatiskt bli sann.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char |  |

### setTreatConsecutiveDelimitersAsOne(boolean value) {#setTreatConsecutiveDelimitersAsOne-boolean-}
```
public void setTreatConsecutiveDelimitersAsOne(boolean value)
```


Om på varandra följande avgränsare ska behandlas som en.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTreatQuotePrefixAsValue(boolean value) {#setTreatQuotePrefixAsValue-boolean-}
```
public void setTreatQuotePrefixAsValue(boolean value)
```


Indikerar om det inledande enkla citattecknet ska tas som en del av värdet i en cell. Standard är sant. Om det är falskt kommer det inledande enkla citattecknet att tas bort från motsvarande cells värde och [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) kommer att sättas till sant för cellen.

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

