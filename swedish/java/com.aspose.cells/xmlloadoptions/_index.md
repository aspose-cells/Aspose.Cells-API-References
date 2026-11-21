---
title: "XmlLoadOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att läsa in xml."
type: docs
url: /sv/java/com.aspose.cells/xmlloadoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LoadOptions](../../com.aspose.cells/loadoptions)
```
public class XmlLoadOptions extends LoadOptions
```

Representerar alternativen för att läsa in xml.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [XmlLoadOptions()](#XmlLoadOptions--) | Representerar alternativen för att läsa in en XML‑fil. |
| [XmlLoadOptions(int type)](#XmlLoadOptions-int-) | Representerar alternativen för att läsa in en XML‑fil. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [containsMultipleWorksheets()](#containsMultipleWorksheets--) | Anger om XML importeras som flera arbetsblad. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Anger om data automatiskt filtreras när filerna laddas. |
| [getAutoFitterOptions()](#getAutoFitterOptions--) | Hämtar auto-fitter-alternativen |
| [getCheckDataValid()](#getCheckDataValid--) | Kontrollera om data är giltiga i mallfilen. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getClass()](#getClass--) |  |
| [getConvertNumericOrDate()](#getConvertNumericOrDate--) | Anger om värdet i XML‑filen konverteras till numeriskt eller datum. |
| [getDateFormat()](#getDateFormat--) | Hämtar formatet för datumvärdet. |
| [getDefaultStyleSettings()](#getDefaultStyleSettings--) | Hämtar standardstilinställningarna för att initiera stilar i arbetsboken |
| [getFontConfigs()](#getFontConfigs--) | Hämtar individuella teckensnittskonfigurationer. |
| [getIgnoreNotPrinted()](#getIgnoreNotPrinted--) | Ignorera data som inte skrivs ut om filen skrivs ut direkt |
| [getIgnoreRootAttributes()](#getIgnoreRootAttributes--) | Anger om attribut i rot‑elementet ska ignoreras. |
| [getIgnoreUselessShapes()](#getIgnoreUselessShapes--) | Anger om onödiga former ska ignoreras. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Hämtar avbrottsövervakaren. |
| [getKeepUnparsedData()](#getKeepUnparsedData--) | Om oparsade data ska behållas i minnet för arbetsboken när den laddas från mallfilen. |
| [getLanguageCode()](#getLanguageCode--) | Hämtar användargränssnittsspråket för arbetsboksversionen baserat på landskoden som har sparat filen. |
| [getLightCellsDataHandler()](#getLightCellsDataHandler--) | Datahanteraren för att bearbeta celldata när mallfilen läses. |
| [getLoadFilter()](#getLoadFilter--) | Filtret som anger hur data ska laddas. |
| [getLoadFormat()](#getLoadFormat--) | Hämtar laddningsformatet. |
| [getLocale()](#getLocale--) | Hämtar de regionala inställningarna som används för arbetsboken som ska laddas. |
| [getMemorySetting()](#getMemorySetting--) | Hämtar minnesläget för den laddade arbetsboken. |
| [getNumberFormat()](#getNumberFormat--) | Hämtar formatet för numeriskt värde. |
| [getParsingFormulaOnOpen()](#getParsingFormulaOnOpen--) | Anger om formeln ska parsas när filen läses. |
| [getParsingPivotCachedRecords()](#getParsingPivotCachedRecords--) | Anger om pivottabellens cachade poster ska parsas när filen laddas. |
| [getPassword()](#getPassword--) | Hämtar arbetsbokens lösenord. |
| [getPreservePaddingSpacesInFormula()](#getPreservePaddingSpacesInFormula--) | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras när formler hämtas och sätts. |
| [getRegion()](#getRegion--) | Hämtar de regionala inställningarna som används för arbetsboken som ska laddas. |
| [getStandardFont()](#getStandardFont--) | Ställer in standardteckensnittets namn |
| [getStandardFontSize()](#getStandardFontSize--) | Ställer in standardteckensnittets storlek. |
| [getStartCell()](#getStartCell--) | Hämtar startcellen. |
| [getWarningCallback()](#getWarningCallback--) | Hämtar varningsåteranrop. |
| [hashCode()](#hashCode--) |  |
| [isXmlMap()](#isXmlMap--) | Anger om XML ska mappas till Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFilter(boolean value)](#setAutoFilter-boolean-) | Anger om data automatiskt filtreras när filerna laddas. |
| [setAutoFitterOptions(AutoFitterOptions value)](#setAutoFitterOptions-com.aspose.cells.AutoFitterOptions-) | Ställer in auto-fitter-alternativen |
| [setCheckDataValid(boolean value)](#setCheckDataValid-boolean-) | Kontrollera om data är giltiga i mallfilen. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setContainsMultipleWorksheets(boolean value)](#setContainsMultipleWorksheets-boolean-) | Anger om XML importeras som flera arbetsblad. |
| [setConvertNumericOrDate(boolean value)](#setConvertNumericOrDate-boolean-) | Anger om värdet i XML‑filen konverteras till numeriskt eller datum. |
| [setDateFormat(String value)](#setDateFormat-java.lang.String-) | Ställer in formatet för datumvärdet. |
| [setFontConfigs(IndividualFontConfigs value)](#setFontConfigs-com.aspose.cells.IndividualFontConfigs-) | Ställer in individuella teckensnittskonfigurationer. |
| [setIgnoreNotPrinted(boolean value)](#setIgnoreNotPrinted-boolean-) | Ignorera data som inte skrivs ut om filen skrivs ut direkt |
| [setIgnoreRootAttributes(boolean value)](#setIgnoreRootAttributes-boolean-) | Anger om attribut i rot‑elementet ska ignoreras. |
| [setIgnoreUselessShapes(boolean value)](#setIgnoreUselessShapes-boolean-) | Anger om onödiga former ska ignoreras. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Ställer in avbrottsövervakaren. |
| [setKeepUnparsedData(boolean value)](#setKeepUnparsedData-boolean-) | Om oparsade data ska behållas i minnet för arbetsboken när den laddas från mallfilen. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Ställer in användargränssnittets språk för Workbook-versionen baserat på CountryCode som har sparat filen. |
| [setLightCellsDataHandler(LightCellsDataHandler value)](#setLightCellsDataHandler-com.aspose.cells.LightCellsDataHandler-) | Datahanteraren för att bearbeta celldata när mallfilen läses. |
| [setLoadFilter(LoadFilter value)](#setLoadFilter-com.aspose.cells.LoadFilter-) | Filtret som anger hur data ska laddas. |
| [setLocale(Locale value)](#setLocale-java.util.Locale-) | Ställer in de regionala inställningarna som används för Workbook som ska laddas. |
| [setMemorySetting(int value)](#setMemorySetting-int-) | Ställer in minnesläget för den laddade arbetsboken. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Ställer in formatet för numeriskt värde. |
| [setPaperSize(int type)](#setPaperSize-int-) | Ställer in standardpappersstorlek för utskrift från standardskrivarens inställning. |
| [setParsingFormulaOnOpen(boolean value)](#setParsingFormulaOnOpen-boolean-) | Anger om formeln ska parsas när filen läses. |
| [setParsingPivotCachedRecords(boolean value)](#setParsingPivotCachedRecords-boolean-) | Anger om pivottabellens cachade poster ska parsas när filen laddas. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Ställer in lösenordet för arbetsboken. |
| [setPreservePaddingSpacesInFormula(boolean value)](#setPreservePaddingSpacesInFormula-boolean-) | Anger om mellanslag och radbrytningar som finns mellan formeltoken ska bevaras när formler hämtas och sätts. |
| [setRegion(int value)](#setRegion-int-) | Ställer in de regionala inställningarna som används för Workbook som ska laddas. |
| [setStandardFont(String value)](#setStandardFont-java.lang.String-) | Ställer in standardteckensnittets namn |
| [setStandardFontSize(double value)](#setStandardFontSize-double-) | Ställer in standardteckensnittets storlek. |
| [setStartCell(String value)](#setStartCell-java.lang.String-) | Ställer in startcellen. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Ställer in varningsåteranrop. |
| [setXmlMap(boolean value)](#setXmlMap-boolean-) | Anger om XML ska mappas till Excel. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### XmlLoadOptions() {#XmlLoadOptions--}
```
public XmlLoadOptions()
```


Representerar alternativen för att läsa in en XML‑fil.

### XmlLoadOptions(int type) {#XmlLoadOptions-int-}
```
public XmlLoadOptions(int type)
```


Representerar alternativen för att läsa in en XML‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [LoadFormat](../../com.aspose.cells/loadformat). Laddningsformatstypen. |

### containsMultipleWorksheets() {#containsMultipleWorksheets--}
```
public boolean containsMultipleWorksheets()
```


Anger om XML importeras som flera arbetsblad.

**Returns:**
boolean
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
### getConvertNumericOrDate() {#getConvertNumericOrDate--}
```
public boolean getConvertNumericOrDate()
```


Anger om värdet i XML‑filen konverteras till numeriskt eller datum.

**Returns:**
boolean
### getDateFormat() {#getDateFormat--}
```
public String getDateFormat()
```


Hämtar formatet för datumvärdet.

**Returns:**
java.lang.String
### getDefaultStyleSettings() {#getDefaultStyleSettings--}
```
public DefaultStyleSettings getDefaultStyleSettings()
```


Hämtar standardstilinställningarna för att initiera stilar i arbetsboken

**Returns:**
[DefaultStyleSettings](../../com.aspose.cells/defaultstylesettings)
### getFontConfigs() {#getFontConfigs--}
```
public IndividualFontConfigs getFontConfigs()
```


Hämtar individuella teckensnittskonfigurationer. Fungerar endast för den [Workbook](../../com.aspose.cells/workbook) som använder dessa [LoadOptions](../../com.aspose.cells/loadoptions) för att laddas.

**Returns:**
[IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs)
### getIgnoreNotPrinted() {#getIgnoreNotPrinted--}
```
public boolean getIgnoreNotPrinted()
```


Ignorera data som inte skrivs ut om filen skrivs ut direkt

**Remarks**

Endast för xlsx-fil.

**Returns:**
boolean
### getIgnoreRootAttributes() {#getIgnoreRootAttributes--}
```
public boolean getIgnoreRootAttributes()
```


Anger om attribut i rot‑elementet ska ignoreras.

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
### getLocale() {#getLocale--}
```
public Locale getLocale()
```


Hämtar de regionala inställningarna som används för arbetsboken som ska laddas.

**Remarks**

Denna egenskap har samma effekt som [getRegion()](../../com.aspose.cells/loadoptions\#getRegion--) för att ställa in regionala inställningar.

**Returns:**
java.util.Locale
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
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Hämtar formatet för numeriskt värde.

**Returns:**
java.lang.String
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
### getStartCell() {#getStartCell--}
```
public String getStartCell()
```


Hämtar startcellen.

**Remarks**

Fungerar endast när filen inte är speadsheetML eller när XML mappas till Excel.

**Returns:**
java.lang.String
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
### isXmlMap() {#isXmlMap--}
```
public boolean isXmlMap()
```


Anger om XML ska mappas till Excel. Standardvärdet är falskt.

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

### setContainsMultipleWorksheets(boolean value) {#setContainsMultipleWorksheets-boolean-}
```
public void setContainsMultipleWorksheets(boolean value)
```


Anger om XML importeras som flera arbetsblad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setConvertNumericOrDate(boolean value) {#setConvertNumericOrDate-boolean-}
```
public void setConvertNumericOrDate(boolean value)
```


Anger om värdet i XML‑filen konverteras till numeriskt eller datum.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setDateFormat(String value) {#setDateFormat-java.lang.String-}
```
public void setDateFormat(String value)
```


Ställer in formatet för datumvärdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFontConfigs(IndividualFontConfigs value) {#setFontConfigs-com.aspose.cells.IndividualFontConfigs-}
```
public void setFontConfigs(IndividualFontConfigs value)
```


Ställer in individuella teckensnittskonfigurationer. Fungerar endast för den [Workbook](../../com.aspose.cells/workbook) som använder dessa [LoadOptions](../../com.aspose.cells/loadoptions) för att läsa in.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IndividualFontConfigs](../../com.aspose.cells/individualfontconfigs) |  |

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

### setIgnoreRootAttributes(boolean value) {#setIgnoreRootAttributes-boolean-}
```
public void setIgnoreRootAttributes(boolean value)
```


Anger om attribut i rot‑elementet ska ignoreras.

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

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Ställer in formatet för numeriskt värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

### setStartCell(String value) {#setStartCell-java.lang.String-}
```
public void setStartCell(String value)
```


Ställer in startcellen.

**Remarks**

Fungerar endast när filen inte är speadsheetML eller när XML mappas till Excel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Ställer in varningsåteranrop.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### setXmlMap(boolean value) {#setXmlMap-boolean-}
```
public void setXmlMap(boolean value)
```


Anger om XML ska mappas till Excel. Standardvärdet är falskt.

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

