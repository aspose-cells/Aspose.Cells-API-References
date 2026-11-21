---
title: "OoxmlSaveOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att spara Office Open XML-fil."
type: docs
url: /sv/java/com.aspose.cells/ooxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class OoxmlSaveOptions extends SaveOptions
```

Representerar alternativen för att spara Office Open XML-fil.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [OoxmlSaveOptions()](#OoxmlSaveOptions--) | Skapar alternativen för att spara Office Open XML‑fil. |
| [OoxmlSaveOptions(int saveFormat)](#OoxmlSaveOptions-int-) | Skapar alternativen för att spara Office Open XML‑fil. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAsFlatOpc()](#getAsFlatOpc--) | Anger om sparning som en platt OPC‑fil som kan genereras av Open XML SDK. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Mappen för temporära filer som kan användas som datacache. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Gör arbetsboken tom efter att filen har sparats. |
| [getCompressionType()](#getCompressionType--) | Hämtar komprimeringstypen för ooxml-filen. |
| [getCreateDirectory()](#getCreateDirectory--) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [getEmbedOoxmlAsOleObject()](#getEmbedOoxmlAsOleObject--) | Anger om Ooxml‑filer för OleObject ska bäddas in som ole‑objekt. |
| [getEnableZip64()](#getEnableZip64--) | Använd ZIP64‑tillägg vid skrivning av zip‑arkiv, vid behov. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [getExportCellName()](#getExportCellName--) | Anger om cellnamn ska exporteras till Excel2007‑filen .xlsx (.xlsm, .xltx, .xltm). |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | Dataleverantören för att spara arbetsbok i lätt läge. |
| [getMergeAreas()](#getMergeAreas--) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Anger om den senaste diagramdata ska cachas. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar filformatet för sparning. |
| [getSortExternalNames()](#getSortExternalNames--) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [getSortNames()](#getSortNames--) | Anger om definierade namn ska sorteras innan filen sparas. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Anger om inställning för SmartArt ska uppdateras. |
| [getUpdateZoom()](#getUpdateZoom--) | Anger om skalningsfaktorn ska uppdateras innan filen sparas om egenskaperna PageSetup.FitToPagesWide och PageSetup.FitToPagesTall styr hur kalkylbladet skalas. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [getWarningCallback()](#getWarningCallback--) | Hämtar varningsåteranrop. |
| [getWpsCompatibility()](#getWpsCompatibility--) | Anger om xls-filen ska göras mer kompatibel med WPS. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAsFlatOpc(boolean value)](#setAsFlatOpc-boolean-) | Anger om sparning som en platt OPC‑fil som kan genereras av Open XML SDK. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Mappen för temporära filer som kan användas som datacache. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setClearData(boolean value)](#setClearData-boolean-) | Gör arbetsboken tom efter att filen har sparats. |
| [setCompressionType(int value)](#setCompressionType-int-) | Ställer in komprimeringstypen för ooxml-filen. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [setEmbedOoxmlAsOleObject(boolean value)](#setEmbedOoxmlAsOleObject-boolean-) | Anger om Ooxml‑filer för OleObject ska bäddas in som ole‑objekt. |
| [setEnableZip64(boolean value)](#setEnableZip64-boolean-) | Använd ZIP64‑tillägg vid skrivning av zip‑arkiv, vid behov. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [setExportCellName(boolean value)](#setExportCellName-boolean-) | Anger om cellnamn ska exporteras till Excel2007‑filen .xlsx (.xlsm, .xltx, .xltm). |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Dataleverantören för att spara arbetsbok i lätt läge. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Anger om den senaste diagramdata ska cachas. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Anger om definierade namn ska sorteras innan filen sparas. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Anger om inställning för SmartArt ska uppdateras. |
| [setUpdateZoom(boolean value)](#setUpdateZoom-boolean-) | Anger om skalningsfaktorn ska uppdateras innan filen sparas om egenskaperna PageSetup.FitToPagesWide och PageSetup.FitToPagesTall styr hur kalkylbladet skalas. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Ställer in varningsåteranrop. |
| [setWpsCompatibility(boolean value)](#setWpsCompatibility-boolean-) | Anger om xls-filen ska göras mer kompatibel med WPS. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### OoxmlSaveOptions() {#OoxmlSaveOptions--}
```
public OoxmlSaveOptions()
```


Skapar alternativen för att spara Office Open XML‑fil.

### OoxmlSaveOptions(int saveFormat) {#OoxmlSaveOptions-int-}
```
public OoxmlSaveOptions(int saveFormat)
```


Skapar alternativen för att spara Office Open XML‑fil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Filformatet. Det bör vara en av följande typer: [SaveFormat.XLSX](../../com.aspose.cells/saveformat\#XLSX), [SaveFormat.XLTX](../../com.aspose.cells/saveformat\#XLTX), [SaveFormat.XLAM](../../com.aspose.cells/saveformat\#XLAM), [SaveFormat.XLSM](../../com.aspose.cells/saveformat\#XLSM) eller [SaveFormat.XLTM](../../com.aspose.cells/saveformat\#XLTM), annars kommer det sparade formatet automatiskt att sättas till [SaveFormat.XLSX](../../com.aspose.cells/saveformat\#XLSX). |

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
### getAsFlatOpc() {#getAsFlatOpc--}
```
public boolean getAsFlatOpc()
```


Anger om sparning som en platt OPC‑fil som kan genereras av Open XML SDK.

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
### getCompressionType() {#getCompressionType--}
```
public int getCompressionType()
```


Hämtar komprimeringstypen för ooxml-filen.

Se [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

Standardvärdet är OoxmlCompressionType.Level2.

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
### getEmbedOoxmlAsOleObject() {#getEmbedOoxmlAsOleObject--}
```
public boolean getEmbedOoxmlAsOleObject()
```


Anger om Ooxml‑filer för OleObject ska bäddas in som ole‑objekt.

**Remarks**

Endast för OleObject.

**Returns:**
boolean
### getEnableZip64() {#getEnableZip64--}
```
public boolean getEnableZip64()
```


Använd ZIP64‑tillägg vid skrivning av zip‑arkiv, vid behov.

**Returns:**
boolean
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```


Anger om dokumentegenskaper ska krypteras vid sparande som .xls-fil. Standardvärdet är sant.

**Remarks**

Endast för .xls, .xlsx, .xlsb och .xlsm-filer.

**Returns:**
boolean
### getExportCellName() {#getExportCellName--}
```
public boolean getExportCellName()
```


Anger om cellnamn ska exporteras till Excel2007‑filen .xlsx (.xlsm, .xltx, .xltm). Om utdatafilen kan nås av SQL Server DTS måste detta värde vara true. Att sätta värdet till false förbättrar prestandan avsevärt och minskar filstorleken när stora filer skapas. Standardvärdet är true.

**Returns:**
boolean
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


Dataleverantören för att spara arbetsbok i lätt läge.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Anger om den senaste diagramdata ska cachas.

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
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Anger om inställning för SmartArt ska uppdateras. Standardvärdet är falskt.

**Remarks**

Påverkar endast efter att ha anropat metoden Shape.GetResultOfSmartArt() och de cachade formerna finns i mallfilen.

**Returns:**
boolean
### getUpdateZoom() {#getUpdateZoom--}
```
public boolean getUpdateZoom()
```


Anger om skalningsfaktorn ska uppdateras innan filen sparas om egenskaperna PageSetup.FitToPagesWide och PageSetup.FitToPagesTall styr hur kalkylbladet skalas.

**Remarks**

Standardvärdet är false för prestanda.

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
### getWpsCompatibility() {#getWpsCompatibility--}
```
public boolean getWpsCompatibility()
```


Anger om xls-filen ska göras mer kompatibel med WPS.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen WorkbookSetting.WpsCompatibility. Denna metod kommer att tas bort 12 månader senare från och med december 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAsFlatOpc(boolean value) {#setAsFlatOpc-boolean-}
```
public void setAsFlatOpc(boolean value)
```


Anger om sparning som en platt OPC‑fil som kan genereras av Open XML SDK.

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

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Gör arbetsboken tom efter att filen har sparats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCompressionType(int value) {#setCompressionType-int-}
```
public void setCompressionType(int value)
```


Ställer in komprimeringstypen för ooxml-filen.

Se [OoxmlCompressionType](../../com.aspose.cells/ooxmlcompressiontype).

**Remarks**

Standardvärdet är OoxmlCompressionType.Level2.

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

### setEmbedOoxmlAsOleObject(boolean value) {#setEmbedOoxmlAsOleObject-boolean-}
```
public void setEmbedOoxmlAsOleObject(boolean value)
```


Anger om Ooxml‑filer för OleObject ska bäddas in som ole‑objekt.

**Remarks**

Endast för OleObject.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEnableZip64(boolean value) {#setEnableZip64-boolean-}
```
public void setEnableZip64(boolean value)
```


Använd ZIP64‑tillägg vid skrivning av zip‑arkiv, vid behov.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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

### setExportCellName(boolean value) {#setExportCellName-boolean-}
```
public void setExportCellName(boolean value)
```


Anger om cellnamn ska exporteras till Excel2007‑filen .xlsx (.xlsm, .xltx, .xltm). Om utdatafilen kan nås av SQL Server DTS måste detta värde vara true. Att sätta värdet till false förbättrar prestandan avsevärt och minskar filstorleken när stora filer skapas. Standardvärdet är true.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


Dataleverantören för att spara arbetsbok i lätt läge.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

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

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Anger om den senaste diagramdata ska cachas.

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

### setUpdateZoom(boolean value) {#setUpdateZoom-boolean-}
```
public void setUpdateZoom(boolean value)
```


Anger om skalningsfaktorn ska uppdateras innan filen sparas om egenskaperna PageSetup.FitToPagesWide och PageSetup.FitToPagesTall styr hur kalkylbladet skalas.

**Remarks**

Standardvärdet är false för prestanda.

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

### setWpsCompatibility(boolean value) {#setWpsCompatibility-boolean-}
```
public void setWpsCompatibility(boolean value)
```


Anger om xls-filen ska göras mer kompatibel med WPS.

**Remarks**

OBS: Denna medlem är nu föråldrad. Använd istället egenskapen WorkbookSetting.WpsCompatibility. Denna metod kommer att tas bort 12 månader senare från och med december 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

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

