---
title: "XmlSaveOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att spara arbetsboken som en xml-fil."
type: docs
url: /sv/java/com.aspose.cells/xmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class XmlSaveOptions extends SaveOptions
```

Representerar alternativen för att spara arbetsboken som en xml-fil.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [XmlSaveOptions()](#XmlSaveOptions--) | Skapar alternativ för att spara xml‑fil. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | Mappen för temporära filer som kan användas som datacache. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Gör arbetsboken tom efter att filen har sparats. |
| [getCreateDirectory()](#getCreateDirectory--) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [getDataAsAttribute()](#getDataAsAttribute--) | Indikerar om data exporteras som attribut för elementet. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [getExportArea()](#getExportArea--) | Hämtar exportintervallet. |
| [getMergeAreas()](#getMergeAreas--) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Anger om den senaste diagramdata ska cachas. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar filformatet för sparning. |
| [getSheetIndexes()](#getSheetIndexes--) | Representerar indexen för exporterade blad. |
| [getSheetNameAsElementName()](#getSheetNameAsElementName--) | Indikerar om bladets namn exporteras som elementets namn. |
| [getSortExternalNames()](#getSortExternalNames--) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [getSortNames()](#getSortNames--) | Anger om definierade namn ska sorteras innan filen sparas. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Anger om inställning för SmartArt ska uppdateras. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [getWarningCallback()](#getWarningCallback--) | Hämtar varningsåteranrop. |
| [getXmlMapName()](#getXmlMapName--) | Indikerar om xml‑kartan exporteras i filen. |
| [hasHeaderRow()](#hasHeaderRow--) | Indikerar om intervallet innehåller rubrikrad. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Mappen för temporära filer som kan användas som datacache. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setClearData(boolean value)](#setClearData-boolean-) | Gör arbetsboken tom efter att filen har sparats. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [setDataAsAttribute(boolean value)](#setDataAsAttribute-boolean-) | Indikerar om data exporteras som attribut för elementet. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Ställer in exportintervallet. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | Indikerar om intervallet innehåller rubrikrad. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Anger om den senaste diagramdata ska cachas. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | Representerar indexen för exporterade blad. |
| [setSheetNameAsElementName(boolean value)](#setSheetNameAsElementName-boolean-) | Indikerar om bladets namn exporteras som elementets namn. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Anger om definierade namn ska sorteras innan filen sparas. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Anger om inställning för SmartArt ska uppdateras. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Ställer in varningsåteranrop. |
| [setXmlMapName(String value)](#setXmlMapName-java.lang.String-) | Indikerar om xml‑kartan exporteras i filen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### XmlSaveOptions() {#XmlSaveOptions--}
```
public XmlSaveOptions()
```


Skapar alternativ för att spara xml‑fil.

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
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getDataAsAttribute() {#getDataAsAttribute--}
```
public boolean getDataAsAttribute()
```


Indikerar om data exporteras som attribut för elementet.

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
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


Hämtar exportintervallet.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
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
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


Representerar indexen för exporterade blad.

**Returns:**
int[]
### getSheetNameAsElementName() {#getSheetNameAsElementName--}
```
public boolean getSheetNameAsElementName()
```


Indikerar om bladets namn exporteras som elementets namn.

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
### getXmlMapName() {#getXmlMapName--}
```
public String getXmlMapName()
```


Indikerar om xml‑kartan exporteras i filen.

**Returns:**
java.lang.String
### hasHeaderRow() {#hasHeaderRow--}
```
public boolean hasHeaderRow()
```


Indikerar om intervallet innehåller rubrikrad.

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

### setDataAsAttribute(boolean value) {#setDataAsAttribute-boolean-}
```
public void setDataAsAttribute(boolean value)
```


Indikerar om data exporteras som attribut för elementet.

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

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Ställer in exportintervallet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


Indikerar om intervallet innehåller rubrikrad.

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

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Anger om den senaste diagramdata ska cachas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


Representerar indexen för exporterade blad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int[] |  |

### setSheetNameAsElementName(boolean value) {#setSheetNameAsElementName-boolean-}
```
public void setSheetNameAsElementName(boolean value)
```


Indikerar om bladets namn exporteras som elementets namn.

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

### setXmlMapName(String value) {#setXmlMapName-java.lang.String-}
```
public void setXmlMapName(String value)
```


Indikerar om xml‑kartan exporteras i filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

