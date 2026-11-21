---
title: "SqlScriptSaveOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att spara sql."
type: docs
url: /sv/java/com.aspose.cells/sqlscriptsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class SqlScriptSaveOptions extends SaveOptions
```

Representerar alternativen för att spara sql.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [SqlScriptSaveOptions()](#SqlScriptSaveOptions--) | Skapar alternativ för att spara sql-fil. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddBlankLineBetweenRows()](#getAddBlankLineBetweenRows--) | Infoga en tom rad mellan varje datapost. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Mappen för temporära filer som kan användas som datacache. |
| [getCheckAllDataForColumnType()](#getCheckAllDataForColumnType--) | Kontrollera all data för att hitta kolumners datatyp. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [getCheckIfTableExists()](#getCheckIfTableExists--) | Kontrollera om tabellnamnet finns innan det skapas |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Gör arbetsboken tom efter att filen har sparats. |
| [getColumnTypeMap()](#getColumnTypeMap--) | Hämtar kartan över kolumntyp för olika databaser. |
| [getCreateDirectory()](#getCreateDirectory--) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [getCreateTable()](#getCreateTable--) | Anger om export av sql för att skapa tabell. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [getExportArea()](#getExportArea--) | Hämtar exportintervallet. |
| [getExportAsString()](#getExportAsString--) | Anger om all data exporteras som strängvärde. |
| [getIdName()](#getIdName--) | Hämtar namnet på id‑kolumnen. |
| [getMergeAreas()](#getMergeAreas--) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [getOperatorType()](#getOperatorType--) | Hämtar operator‑typen för sql. |
| [getPrimaryKey()](#getPrimaryKey--) | Representerar vilken kolumn som är primärnyckel i datatabellen. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Anger om den senaste diagramdata ska cachas. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar filformatet för sparning. |
| [getSeparator()](#getSeparator--) | Hämtar teckenseparatorn för sql‑skriptet. |
| [getSheetIndexes()](#getSheetIndexes--) | Representerar indexen för exporterade blad. |
| [getSortExternalNames()](#getSortExternalNames--) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [getSortNames()](#getSortNames--) | Anger om definierade namn ska sorteras innan filen sparas. |
| [getStartId()](#getStartId--) | Hämtar start‑id:t. |
| [getTableName()](#getTableName--) | Hämtar tabellnamnet. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Anger om inställning för SmartArt ska uppdateras. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [getWarningCallback()](#getWarningCallback--) | Hämtar varningsåteranrop. |
| [hasHeaderRow()](#hasHeaderRow--) | Indikerar om intervallet innehåller rubrikrad. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddBlankLineBetweenRows(boolean value)](#setAddBlankLineBetweenRows-boolean-) | Infoga en tom rad mellan varje datapost. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Mappen för temporära filer som kan användas som datacache. |
| [setCheckAllDataForColumnType(boolean value)](#setCheckAllDataForColumnType-boolean-) | Kontrollera all data för att hitta kolumners datatyp. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Om restriktioner för Excel-filen ska kontrolleras när användaren modifierar cellrelaterade objekt. |
| [setCheckIfTableExists(boolean value)](#setCheckIfTableExists-boolean-) | Kontrollera om tabellnamnet finns innan det skapas |
| [setClearData(boolean value)](#setClearData-boolean-) | Gör arbetsboken tom efter att filen har sparats. |
| [setColumnTypeMap(SqlScriptColumnTypeMap value)](#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-) | Ställer in mappningen av kolumntyp för olika databaser. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas. |
| [setCreateTable(boolean value)](#setCreateTable-boolean-) | Anger om export av sql för att skapa tabell. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Anger om dokumentegenskaper ska krypteras när filen sparas som .xls. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Ställer in exportintervallet. |
| [setExportAsString(boolean value)](#setExportAsString-boolean-) | Anger om all data exporteras som strängvärde. |
| [setHasHeaderRow(boolean value)](#setHasHeaderRow-boolean-) | Indikerar om intervallet innehåller rubrikrad. |
| [setIdName(String value)](#setIdName-java.lang.String-) | Ställer in namnet på id‑kolumnen. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas. |
| [setOperatorType(int value)](#setOperatorType-int-) | Ställer in operator‑typen för sql. |
| [setPrimaryKey(int value)](#setPrimaryKey-int-) | Representerar vilken kolumn som är primärnyckel i datatabellen. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Anger om den senaste diagramdata ska cachas. |
| [setSeparator(char value)](#setSeparator-char-) | Ställer in teckenseparatorn för sql‑skriptet. |
| [setSheetIndexes(int[] value)](#setSheetIndexes-int---) | Representerar indexen för exporterade blad. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Anger om externa definierade namn ska sorteras innan filen sparas. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Anger om definierade namn ska sorteras innan filen sparas. |
| [setStartId(int value)](#setStartId-int-) | Ställer in start‑id:t. |
| [setTableName(String value)](#setTableName-java.lang.String-) | Ställer in tabellnamnet. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Anger om inställning för SmartArt ska uppdateras. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Anger om sammanslagna celler ska valideras innan filen sparas. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Ställer in varningsåteranrop. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SqlScriptSaveOptions() {#SqlScriptSaveOptions--}
```
public SqlScriptSaveOptions()
```


Skapar alternativ för att spara sql-fil.

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
### getAddBlankLineBetweenRows() {#getAddBlankLineBetweenRows--}
```
public boolean getAddBlankLineBetweenRows()
```


Infoga en tom rad mellan varje datapost.

**Remarks**

Om [getSeparator()](../../com.aspose.cells/sqlscriptsaveoptions\#getSeparator--) är '\\n' , är det bättre att sätta denna egenskap till true för att öka läsbarheten.

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
### getCheckAllDataForColumnType() {#getCheckAllDataForColumnType--}
```
public boolean getCheckAllDataForColumnType()
```


Kontrollera all data för att hitta kolumners datatyp.

**Remarks**

Standardvärdet är false, vi kontrollerar bara den första raden för prestanda. Om denna egenskap är true och kolumnerna innehåller blandade värdetyper, kommer kolumnernas typ att vara text.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Om kontroll av begränsningar i Excel-filen när användaren ändrar cellrelaterade objekt. Till exempel tillåter Excel inte att ange ett strängvärde längre än 32K. När du anger ett värde som är längre än 32K trunkeras det.

**Returns:**
boolean
### getCheckIfTableExists() {#getCheckIfTableExists--}
```
public boolean getCheckIfTableExists()
```


Kontrollera om tabellnamnet finns innan det skapas

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
### getColumnTypeMap() {#getColumnTypeMap--}
```
public SqlScriptColumnTypeMap getColumnTypeMap()
```


Hämtar kartan över kolumntyp för olika databaser.

**Returns:**
[SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap)
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Om true och katalogen inte finns, kommer katalogen att automatiskt skapas innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getCreateTable() {#getCreateTable--}
```
public boolean getCreateTable()
```


Anger om export av sql för att skapa tabell.

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
### getExportAsString() {#getExportAsString--}
```
public boolean getExportAsString()
```


Anger om all data exporteras som strängvärde.

**Returns:**
boolean
### getIdName() {#getIdName--}
```
public String getIdName()
```


Hämtar namnet på id‑kolumnen.

**Remarks**

Om denna egenskap är inställd, kommer en kolumn att infogas med automatiskt ökande heltalsvärde.

**Returns:**
java.lang.String
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Anger om områdena för villkorsstyrd formatering och validering ska slås ihop innan filen sparas.

**Remarks**

Standardvärdet är falskt.

**Returns:**
boolean
### getOperatorType() {#getOperatorType--}
```
public int getOperatorType()
```


Hämtar operator‑typen för sql.

Se [SqlScriptOperatorType](../../com.aspose.cells/sqlscriptoperatortype).

**Returns:**
int
### getPrimaryKey() {#getPrimaryKey--}
```
public int getPrimaryKey()
```


Representerar vilken kolumn som är primärnyckel i datatabellen.

**Returns:**
int
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
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Hämtar teckenseparatorn för sql‑skriptet.

**Remarks**

Kan endast vara ' ' eller '\\n'. Om

**Returns:**
char
### getSheetIndexes() {#getSheetIndexes--}
```
public int[] getSheetIndexes()
```


Representerar indexen för exporterade blad.

**Returns:**
int[]
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
### getStartId() {#getStartId--}
```
public int getStartId()
```


Hämtar start‑id:t.

**Remarks**

Fungerar endast när [getIdName()](../../com.aspose.cells/sqlscriptsaveoptions\#getIdName--) är inställd.

**Returns:**
int
### getTableName() {#getTableName--}
```
public String getTableName()
```


Hämtar tabellnamnet.

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




### setAddBlankLineBetweenRows(boolean value) {#setAddBlankLineBetweenRows-boolean-}
```
public void setAddBlankLineBetweenRows(boolean value)
```


Infoga en tom rad mellan varje datapost.

**Remarks**

Om [getSeparator()](../../com.aspose.cells/sqlscriptsaveoptions\#getSeparator--) är '\\n' , är det bättre att sätta denna egenskap till true för att öka läsbarheten.

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

### setCheckAllDataForColumnType(boolean value) {#setCheckAllDataForColumnType-boolean-}
```
public void setCheckAllDataForColumnType(boolean value)
```


Kontrollera all data för att hitta kolumners datatyp.

**Remarks**

Standardvärdet är false, vi kontrollerar bara den första raden för prestanda. Om denna egenskap är true och kolumnerna innehåller blandade värdetyper, kommer kolumnernas typ att vara text.

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

### setCheckIfTableExists(boolean value) {#setCheckIfTableExists-boolean-}
```
public void setCheckIfTableExists(boolean value)
```


Kontrollera om tabellnamnet finns innan det skapas

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

### setColumnTypeMap(SqlScriptColumnTypeMap value) {#setColumnTypeMap-com.aspose.cells.SqlScriptColumnTypeMap-}
```
public void setColumnTypeMap(SqlScriptColumnTypeMap value)
```


Ställer in mappningen av kolumntyp för olika databaser.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [SqlScriptColumnTypeMap](../../com.aspose.cells/sqlscriptcolumntypemap) |  |

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

### setCreateTable(boolean value) {#setCreateTable-boolean-}
```
public void setCreateTable(boolean value)
```


Anger om export av sql för att skapa tabell.

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

### setExportAsString(boolean value) {#setExportAsString-boolean-}
```
public void setExportAsString(boolean value)
```


Anger om all data exporteras som strängvärde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasHeaderRow(boolean value) {#setHasHeaderRow-boolean-}
```
public void setHasHeaderRow(boolean value)
```


Indikerar om intervallet innehåller rubrikrad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setIdName(String value) {#setIdName-java.lang.String-}
```
public void setIdName(String value)
```


Ställer in namnet på id‑kolumnen.

**Remarks**

Om denna egenskap är inställd, kommer en kolumn att infogas med automatiskt ökande heltalsvärde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

### setOperatorType(int value) {#setOperatorType-int-}
```
public void setOperatorType(int value)
```


Ställer in operator‑typen för sql.

Se [SqlScriptOperatorType](../../com.aspose.cells/sqlscriptoperatortype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPrimaryKey(int value) {#setPrimaryKey-int-}
```
public void setPrimaryKey(int value)
```


Representerar vilken kolumn som är primärnyckel i datatabellen.

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

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Ställer in teckenseparatorn för sql‑skriptet.

**Remarks**

Kan endast vara ' ' eller '\\n'. Om

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | char |  |

### setSheetIndexes(int[] value) {#setSheetIndexes-int---}
```
public void setSheetIndexes(int[] value)
```


Representerar indexen för exporterade blad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int[] |  |

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

### setStartId(int value) {#setStartId-int-}
```
public void setStartId(int value)
```


Ställer in start‑id:t.

**Remarks**

Fungerar endast när [getIdName()](../../com.aspose.cells/sqlscriptsaveoptions\#getIdName--) är inställd.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTableName(String value) {#setTableName-java.lang.String-}
```
public void setTableName(String value)
```


Ställer in tabellnamnet.

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

