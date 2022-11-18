---
title: TxtSaveOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the save options for csv/tab delimited/other text format.
type: docs
weight: 616
url: /java/com.aspose.cells/txtsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class TxtSaveOptions extends SaveOptions
```

Represents the save options for csv/tab delimited/other text format.
## Constructors

| Constructor | Description |
| --- | --- |
| [TxtSaveOptions()](#TxtSaveOptions--) | Creates text file save options. |
| [TxtSaveOptions(int format)](#TxtSaveOptions-int-) | Creates text file save options. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysQuoted()](#getAlwaysQuoted--) | Indicates whether always adding '"' for each field. |
| [getCachedFileFolder()](#getCachedFileFolder--) | The cached file folder is used to store some large data. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getEncoding()](#getEncoding--) | Gets and sets the default encoding. |
| [getExportAllSheets()](#getExportAllSheets--) | Indicates whether exporting all sheets to the text file. |
| [getExportArea()](#getExportArea--) | The range of cells to be exported. |
| [getExportQuotePrefix()](#getExportQuotePrefix--) | Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) is true for it. |
| [getFormatStrategy()](#getFormatStrategy--) | Gets and sets the format strategy when exporting the cell value as string. |
| [getKeepSeparatorsForBlankRow()](#getKeepSeparatorsForBlankRow--) | Indicates whether separators should be output for blank row. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | The Data provider to provide cells data for saving workbook in light mode. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getQuoteType()](#getQuoteType--) | Gets or sets how to quote values in the exported text file. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSeparator()](#getSeparator--) | Gets and sets char Delimiter of text file. |
| [getSeparatorString()](#getSeparatorString--) | Gets and sets a string value as separator. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getTrimLeadingBlankRowAndColumn()](#getTrimLeadingBlankRowAndColumn--) | Indicates whether leading blank rows and columns should be trimmed like what ms excel does. |
| [getTrimTailingBlankCells()](#getTrimTailingBlankCells--) | Indicates whether tailing blank cells in one row should be trimmed. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | Gets or sets warning callback. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysQuoted(boolean value)](#setAlwaysQuoted-boolean-) | Please see the getter of this property: [getAlwaysQuoted()](../../com.aspose.cells/txtsaveoptions\#getAlwaysQuoted--) |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Please see the getter of this property: @CREF1852\_ |
| [setClearData(boolean value)](#setClearData-boolean-) | Please see the getter of this property: @CREF1851\_ |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Please see the getter of this property: @CREF1855\_ |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Please see the getter of this property: [getEncoding()](../../com.aspose.cells/txtsaveoptions\#getEncoding--) |
| [setExportAllSheets(boolean value)](#setExportAllSheets-boolean-) | Please see the getter of this property: [getExportAllSheets()](../../com.aspose.cells/txtsaveoptions\#getExportAllSheets--) |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | Please see the getter of this property: [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) |
| [setExportQuotePrefix(boolean value)](#setExportQuotePrefix-boolean-) | Please see the getter of this property: [getExportQuotePrefix()](../../com.aspose.cells/txtsaveoptions\#getExportQuotePrefix--) |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Please see the getter of this property: [getFormatStrategy()](../../com.aspose.cells/txtsaveoptions\#getFormatStrategy--) |
| [setKeepSeparatorsForBlankRow(boolean value)](#setKeepSeparatorsForBlankRow-boolean-) | Please see the getter of this property: [getKeepSeparatorsForBlankRow()](../../com.aspose.cells/txtsaveoptions\#getKeepSeparatorsForBlankRow--) |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | Please see the getter of this property: [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Please see the getter of this property: @CREF1854\_ |
| [setQuoteType(int value)](#setQuoteType-int-) | Please see the getter of this property: [getQuoteType()](../../com.aspose.cells/txtsaveoptions\#getQuoteType--) |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Please see the getter of this property: @CREF1858\_ |
| [setSeparator(char value)](#setSeparator-char-) | Please see the getter of this property: [getSeparator()](../../com.aspose.cells/txtsaveoptions\#getSeparator--) |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Please see the getter of this property: [getSeparatorString()](../../com.aspose.cells/txtsaveoptions\#getSeparatorString--) |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Please see the getter of this property: @CREF1857\_ |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Please see the getter of this property: @CREF1856\_ |
| [setTrimLeadingBlankRowAndColumn(boolean value)](#setTrimLeadingBlankRowAndColumn-boolean-) | Please see the getter of this property: [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) |
| [setTrimTailingBlankCells(boolean value)](#setTrimTailingBlankCells-boolean-) | Please see the getter of this property: [getTrimTailingBlankCells()](../../com.aspose.cells/txtsaveoptions\#getTrimTailingBlankCells--) |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Please see the getter of this property: @CREF1860\_ |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Please see the getter of this property: @CREF1853\_ |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtSaveOptions() {#TxtSaveOptions--}
```
public TxtSaveOptions()
```


Creates text file save options.

### TxtSaveOptions(int format) {#TxtSaveOptions-int-}
```
public TxtSaveOptions(int format)
```


Creates text file save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | The save format of the text file. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAlwaysQuoted() {#getAlwaysQuoted--}
```
public boolean getAlwaysQuoted()
```


Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will only be quoted when needed(for example, when values contain special characters such as '"' , '\\n' or separator character). Default is false. NOTE: This member is now obsolete. Instead, please use QuoteType property instead. This property will be removed 12 months later since August 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


The cached file folder is used to store some large data.

**Returns:**
java.lang.String
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


Make the workbook empty after saving the file.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Gets and sets the default encoding.

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getExportAllSheets() {#getExportAllSheets--}
```
public boolean getExportAllSheets()
```


Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. The defult value is false.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```


The range of cells to be exported. If the exported area has been specified, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) will takes no effect.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getExportQuotePrefix() {#getExportQuotePrefix--}
```
public boolean getExportQuotePrefix()
```


Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) is true for it. Default is false.

**Returns:**
boolean
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


Gets and sets the format strategy when exporting the cell value as string.

**Returns:**
int
### getKeepSeparatorsForBlankRow() {#getKeepSeparatorsForBlankRow--}
```
public boolean getKeepSeparatorsForBlankRow()
```


Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty.

**Returns:**
boolean
### getLightCellsDataProvider() {#getLightCellsDataProvider--}
```
public LightCellsDataProvider getLightCellsDataProvider()
```


The Data provider to provide cells data for saving workbook in light mode.

**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Returns:**
boolean
### getQuoteType() {#getQuoteType--}
```
public int getQuoteType()
```


Gets or sets how to quote values in the exported text file.

**Returns:**
int
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Indicates whether refreshing chart cache data

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Gets the save file format.

**Returns:**
int
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```


Gets and sets char Delimiter of text file.

**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```


Gets and sets a string value as separator.

**Returns:**
java.lang.String
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```


Indicates whether sorting external defined names before saving file.

**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Indicates whether sorting defined names before saving file.

**Returns:**
boolean
### getTrimLeadingBlankRowAndColumn() {#getTrimLeadingBlankRowAndColumn--}
```
public boolean getTrimLeadingBlankRowAndColumn()
```


Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) or by speicifing [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--)

**Returns:**
boolean
### getTrimTailingBlankCells() {#getTrimTailingBlankCells--}
```
public boolean getTrimTailingBlankCells()
```


Indicates whether tailing blank cells in one row should be trimmed. Default is false. When saving with LightCells mode and the [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--)

**Returns:**
boolean
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indicates whether validate merged cells before saving the file. The default value is false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Gets or sets warning callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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




### setAlwaysQuoted(boolean value) {#setAlwaysQuoted-boolean-}
```
public void setAlwaysQuoted(boolean value)
```


Please see the getter of this property: [getAlwaysQuoted()](../../com.aspose.cells/txtsaveoptions\#getAlwaysQuoted--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Please see the getter of this property: @CREF1852\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Please see the getter of this property: @CREF1851\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Please see the getter of this property: @CREF1855\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```


Please see the getter of this property: [getEncoding()](../../com.aspose.cells/txtsaveoptions\#getEncoding--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setExportAllSheets(boolean value) {#setExportAllSheets-boolean-}
```
public void setExportAllSheets(boolean value)
```


Please see the getter of this property: [getExportAllSheets()](../../com.aspose.cells/txtsaveoptions\#getExportAllSheets--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```


Please see the getter of this property: [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |

### setExportQuotePrefix(boolean value) {#setExportQuotePrefix-boolean-}
```
public void setExportQuotePrefix(boolean value)
```


Please see the getter of this property: [getExportQuotePrefix()](../../com.aspose.cells/txtsaveoptions\#getExportQuotePrefix--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


Please see the getter of this property: [getFormatStrategy()](../../com.aspose.cells/txtsaveoptions\#getFormatStrategy--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setKeepSeparatorsForBlankRow(boolean value) {#setKeepSeparatorsForBlankRow-boolean-}
```
public void setKeepSeparatorsForBlankRow(boolean value)
```


Please see the getter of this property: [getKeepSeparatorsForBlankRow()](../../com.aspose.cells/txtsaveoptions\#getKeepSeparatorsForBlankRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```


Please see the getter of this property: [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Please see the getter of this property: @CREF1854\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setQuoteType(int value) {#setQuoteType-int-}
```
public void setQuoteType(int value)
```


Please see the getter of this property: [getQuoteType()](../../com.aspose.cells/txtsaveoptions\#getQuoteType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Please see the getter of this property: @CREF1858\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```


Please see the getter of this property: [getSeparator()](../../com.aspose.cells/txtsaveoptions\#getSeparator--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |

### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```


Please see the getter of this property: [getSeparatorString()](../../com.aspose.cells/txtsaveoptions\#getSeparatorString--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


Please see the getter of this property: @CREF1857\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Please see the getter of this property: @CREF1856\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTrimLeadingBlankRowAndColumn(boolean value) {#setTrimLeadingBlankRowAndColumn-boolean-}
```
public void setTrimLeadingBlankRowAndColumn(boolean value)
```


Please see the getter of this property: [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTrimTailingBlankCells(boolean value) {#setTrimTailingBlankCells-boolean-}
```
public void setTrimTailingBlankCells(boolean value)
```


Please see the getter of this property: [getTrimTailingBlankCells()](../../com.aspose.cells/txtsaveoptions\#getTrimTailingBlankCells--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


Please see the getter of this property: @CREF1860\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Please see the getter of this property: @CREF1853\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```




**Parameters:**
| Parameter | Type | Description |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

