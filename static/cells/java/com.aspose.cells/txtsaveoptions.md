##TxtSaveOptions
Represents the save options for csv/tab delimited/other text format.
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
| [TxtSaveOptions(int saveFormat)](#TxtSaveOptions-int-) | Creates text file save options. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlwaysQuoted()](#getAlwaysQuoted--) | Indicates whether always adding '"' for each field. |
| [getCachedFileFolder()](#getCachedFileFolder--) | The folder for temporary files that may be used as data cache. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getEncoding()](#getEncoding--) | Gets the default encoding. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indicates whether encrypt document properties when saving as .xls file. |
| [getExportAllSheets()](#getExportAllSheets--) | Indicates whether exporting all sheets to the text file. |
| [getExportArea()](#getExportArea--) | The range of cells to be exported. |
| [getExportQuotePrefix()](#getExportQuotePrefix--) | Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) is true for it. |
| [getFormatStrategy()](#getFormatStrategy--) | Gets the format strategy when exporting the cell value as string. |
| [getKeepSeparatorsForBlankRow()](#getKeepSeparatorsForBlankRow--) | Indicates whether separators should be output for blank row. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--) | The data provider for saving workbook in light mode. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getQuoteType()](#getQuoteType--) | Gets how to quote values in the exported text file. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSeparator()](#getSeparator--) | Gets char Delimiter of text file. |
| [getSeparatorString()](#getSeparatorString--) | Gets a string value as separator. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getTrimLeadingBlankRowAndColumn()](#getTrimLeadingBlankRowAndColumn--) | Indicates whether leading blank rows and columns should be trimmed like what ms excel does. |
| [getTrimTailingBlankCells()](#getTrimTailingBlankCells--) | Indicates whether tailing blank cells in one row should be trimmed. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | Gets warning callback. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlwaysQuoted(boolean value)](#setAlwaysQuoted-boolean-) | Indicates whether always adding '"' for each field. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | The folder for temporary files that may be used as data cache. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Whether check restriction of excel file when user modify cells related objects. |
| [setClearData(boolean value)](#setClearData-boolean-) | Make the workbook empty after saving the file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.cells.Encoding-) | Sets the default encoding. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indicates whether encrypt document properties when saving as .xls file. |
| [setExportAllSheets(boolean value)](#setExportAllSheets-boolean-) | Indicates whether exporting all sheets to the text file. |
| [setExportArea(CellArea value)](#setExportArea-com.aspose.cells.CellArea-) | The range of cells to be exported. |
| [setExportQuotePrefix(boolean value)](#setExportQuotePrefix-boolean-) | Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) is true for it. |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | Sets the format strategy when exporting the cell value as string. |
| [setKeepSeparatorsForBlankRow(boolean value)](#setKeepSeparatorsForBlankRow-boolean-) | Indicates whether separators should be output for blank row. |
| [setLightCellsDataProvider(LightCellsDataProvider value)](#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-) | The data provider for saving workbook in light mode. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setQuoteType(int value)](#setQuoteType-int-) | Sets how to quote values in the exported text file. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indicates whether refreshing chart cache data |
| [setSeparator(char value)](#setSeparator-char-) | Sets char Delimiter of text file. |
| [setSeparatorString(String value)](#setSeparatorString-java.lang.String-) | Sets a string value as separator. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indicates whether sorting external defined names before saving file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indicates whether sorting defined names before saving file. |
| [setTrimLeadingBlankRowAndColumn(boolean value)](#setTrimLeadingBlankRowAndColumn-boolean-) | Indicates whether leading blank rows and columns should be trimmed like what ms excel does. |
| [setTrimTailingBlankCells(boolean value)](#setTrimTailingBlankCells-boolean-) | Indicates whether tailing blank cells in one row should be trimmed. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indicates whether updating smart art setting. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indicates whether validate merged cells before saving the file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Sets warning callback. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### TxtSaveOptions() {#TxtSaveOptions--}
```
public TxtSaveOptions()
```
Creates text file save options.
### TxtSaveOptions(int saveFormat) {#TxtSaveOptions-int-}
```
public TxtSaveOptions(int saveFormat)
```
Creates text file save options.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). The file format. It should be [SaveFormat.CSV](../../com.aspose.cells/saveformat\#CSV) or [SaveFormat.TSV](../../com.aspose.cells/saveformat\#TSV), otherwise the saved format will be set as [SaveFormat.CSV](../../com.aspose.cells/saveformat\#CSV) automatically. |
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
Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will only be quoted when needed(for example, when values contain special characters such as '"' , '\\n' or separator character). Default is false.
**Remarks**
NOTE: This member is now obsolete. Instead, please use QuoteType property instead. This property will be removed 12 months later since August 2012. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```
The folder for temporary files that may be used as data cache.
**Remarks**
If the folder has not been specified, the default value for it is void
**Returns:**
java.lang.String
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.
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
Make the workbook empty after saving the file.
**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```
If true and the directory does not exist, the directory will be automatically created before saving the file.
**Remarks**
The default value is false.
**Returns:**
boolean
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```
Gets the default encoding.
**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```
Indicates whether encrypt document properties when saving as .xls file. The default value is true.
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
**Returns:**
boolean
### getExportAllSheets() {#getExportAllSheets--}
```
public boolean getExportAllSheets()
```
Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel.
**Remarks**
The defult value is false.
**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public CellArea getExportArea()
```
The range of cells to be exported.
**Remarks**
If the exported area has been specified, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) will takes no effect.
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
Gets the format strategy when exporting the cell value as string.
See [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).
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
The data provider for saving workbook in light mode.
**Returns:**
[LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```
Indicates whether merge the areas of conditional formatting and validation before saving the file.
**Remarks**
The default value is false.
**Returns:**
boolean
### getQuoteType() {#getQuoteType--}
```
public int getQuoteType()
```
Gets how to quote values in the exported text file.
See [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).
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
See [SaveFormat](../../com.aspose.cells/saveformat).
**Returns:**
int
### getSeparator() {#getSeparator--}
```
public char getSeparator()
```
Gets char Delimiter of text file.
**Returns:**
char
### getSeparatorString() {#getSeparatorString--}
```
public String getSeparatorString()
```
Gets a string value as separator.
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
Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true.
**Remarks**
Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) or by speicifing [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--)
**Returns:**
boolean
### getTrimTailingBlankCells() {#getTrimTailingBlankCells--}
```
public boolean getTrimTailingBlankCells()
```
Indicates whether tailing blank cells in one row should be trimmed. Default is false.
**Remarks**
When saving with LightCells mode and the [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--)
**Returns:**
boolean
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```
Indicates whether updating smart art setting. The default value is false.
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```
Indicates whether validate merged cells before saving the file.
**Remarks**
The default value is false.
**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```
Gets warning callback.
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
Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will only be quoted when needed(for example, when values contain special characters such as '"' , '\\n' or separator character). Default is false.
**Remarks**
NOTE: This member is now obsolete. Instead, please use QuoteType property instead. This property will be removed 12 months later since August 2012. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```
The folder for temporary files that may be used as data cache.
**Remarks**
If the folder has not been specified, the default value for it is void
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```
Make the workbook empty after saving the file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```
If true and the directory does not exist, the directory will be automatically created before saving the file.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEncoding(Encoding value) {#setEncoding-com.aspose.cells.Encoding-}
```
public void setEncoding(Encoding value)
```
Sets the default encoding.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |
### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```
Indicates whether encrypt document properties when saving as .xls file. The default value is true.
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportAllSheets(boolean value) {#setExportAllSheets-boolean-}
```
public void setExportAllSheets(boolean value)
```
Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel.
**Remarks**
The defult value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportArea(CellArea value) {#setExportArea-com.aspose.cells.CellArea-}
```
public void setExportArea(CellArea value)
```
The range of cells to be exported.
**Remarks**
If the exported area has been specified, [getTrimLeadingBlankRowAndColumn()](../../com.aspose.cells/txtsaveoptions\#getTrimLeadingBlankRowAndColumn--) will takes no effect.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../../com.aspose.cells/cellarea) |  |
### setExportQuotePrefix(boolean value) {#setExportQuotePrefix-boolean-}
```
public void setExportQuotePrefix(boolean value)
```
Indicates whether the single quote sign should be exported as part of the value of one cell when [Style.getQuotePrefix()](../../com.aspose.cells/style\#getQuotePrefix--) is true for it. Default is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```
Sets the format strategy when exporting the cell value as string.
See [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setKeepSeparatorsForBlankRow(boolean value) {#setKeepSeparatorsForBlankRow-boolean-}
```
public void setKeepSeparatorsForBlankRow(boolean value)
```
Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setLightCellsDataProvider(LightCellsDataProvider value) {#setLightCellsDataProvider-com.aspose.cells.LightCellsDataProvider-}
```
public void setLightCellsDataProvider(LightCellsDataProvider value)
```
The data provider for saving workbook in light mode.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataProvider](../../com.aspose.cells/lightcellsdataprovider) |  |
### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```
Indicates whether merge the areas of conditional formatting and validation before saving the file.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setQuoteType(int value) {#setQuoteType-int-}
```
public void setQuoteType(int value)
```
Sets how to quote values in the exported text file.
See [TxtValueQuoteType](../../com.aspose.cells/txtvaluequotetype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```
Indicates whether refreshing chart cache data
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSeparator(char value) {#setSeparator-char-}
```
public void setSeparator(char value)
```
Sets char Delimiter of text file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char |  |
### setSeparatorString(String value) {#setSeparatorString-java.lang.String-}
```
public void setSeparatorString(String value)
```
Sets a string value as separator.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```
Indicates whether sorting external defined names before saving file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```
Indicates whether sorting defined names before saving file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setTrimLeadingBlankRowAndColumn(boolean value) {#setTrimLeadingBlankRowAndColumn-boolean-}
```
public void setTrimLeadingBlankRowAndColumn(boolean value)
```
Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true.
**Remarks**
Same with the rule in ms excel, a row/column will not be taken as blank if it has custom style, even if it contains no cell data. When saving with LightCells mode, this option takes no effect. User should control the output range by the implementation of [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--) or by speicifing [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--)
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setTrimTailingBlankCells(boolean value) {#setTrimTailingBlankCells-boolean-}
```
public void setTrimTailingBlankCells(boolean value)
```
Indicates whether tailing blank cells in one row should be trimmed. Default is false.
**Remarks**
When saving with LightCells mode and the [getExportArea()](../../com.aspose.cells/txtsaveoptions\#getExportArea--) has not been specified, this option takes no effect and one row will be extended to just the last cell provided by the implementation [getLightCellsDataProvider()](../../com.aspose.cells/txtsaveoptions\#getLightCellsDataProvider--)
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```
Indicates whether updating smart art setting. The default value is false.
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```
Indicates whether validate merged cells before saving the file.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```
Sets warning callback.
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
