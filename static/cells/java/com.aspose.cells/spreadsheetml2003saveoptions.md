##SpreadsheetML2003SaveOptions
Represents the options for saving Excel 2003 spreadml file.
**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions)
```
public class SpreadsheetML2003SaveOptions extends SaveOptions
```
Represents the options for saving Excel 2003 spreadml file.
## Constructors
| Constructor | Description |
| --- | --- |
| [SpreadsheetML2003SaveOptions()](#SpreadsheetML2003SaveOptions--) | Creates the options for saving Excel 2003 spreadml file. |
| [SpreadsheetML2003SaveOptions(int saveFormat)](#SpreadsheetML2003SaveOptions-int-) | Creates the options for saving Excel 2003 spreadml file. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCachedFileFolder()](#getCachedFileFolder--) | The folder for temporary files that may be used as data cache. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indicates whether encrypt document properties when saving as .xls file. |
| [getExportColumnIndexOfCell()](#getExportColumnIndexOfCell--) | The default value is false, it means that column index will be ignored if the cell is contiguous to the previous cell. |
| [getLimitAsXls()](#getLimitAsXls--) | Limit as xls, the max row index is 65535 and the max column index is 255. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | Gets warning callback. |
| [hashCode()](#hashCode--) |  |
| [isIndentedFormatting()](#isIndentedFormatting--) | Causes child elements to be indented. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | The folder for temporary files that may be used as data cache. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Whether check restriction of excel file when user modify cells related objects. |
| [setClearData(boolean value)](#setClearData-boolean-) | Make the workbook empty after saving the file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indicates whether encrypt document properties when saving as .xls file. |
| [setExportColumnIndexOfCell(boolean value)](#setExportColumnIndexOfCell-boolean-) | The default value is false, it means that column index will be ignored if the cell is contiguous to the previous cell. |
| [setIndentedFormatting(boolean value)](#setIndentedFormatting-boolean-) | Causes child elements to be indented. |
| [setLimitAsXls(boolean value)](#setLimitAsXls-boolean-) | Limit as xls, the max row index is 65535 and the max column index is 255. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indicates whether refreshing chart cache data |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indicates whether sorting external defined names before saving file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indicates whether sorting defined names before saving file. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indicates whether updating smart art setting. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indicates whether validate merged cells before saving the file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Sets warning callback. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SpreadsheetML2003SaveOptions() {#SpreadsheetML2003SaveOptions--}
```
public SpreadsheetML2003SaveOptions()
```
Creates the options for saving Excel 2003 spreadml file.
### SpreadsheetML2003SaveOptions(int saveFormat) {#SpreadsheetML2003SaveOptions-int-}
```
public SpreadsheetML2003SaveOptions(int saveFormat)
```
Creates the options for saving Excel 2003 spreadml file.
**Remarks**
NOTE: This constructor is now obsolete. Instead, please use SpreadsheetML2003SaveOptions() constructor. This property will be removed 12 months later since January 2021. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). The save format. |
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
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```
Indicates whether encrypt document properties when saving as .xls file. The default value is true.
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
**Returns:**
boolean
### getExportColumnIndexOfCell() {#getExportColumnIndexOfCell--}
```
public boolean getExportColumnIndexOfCell()
```
The default value is false, it means that column index will be ignored if the cell is contiguous to the previous cell.
**Returns:**
boolean
### getLimitAsXls() {#getLimitAsXls--}
```
public boolean getLimitAsXls()
```
Limit as xls, the max row index is 65535 and the max column index is 255.
**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```
Indicates whether merge the areas of conditional formatting and validation before saving the file.
**Remarks**
The default value is false.
**Returns:**
boolean
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
### isIndentedFormatting() {#isIndentedFormatting--}
```
public boolean isIndentedFormatting()
```
Causes child elements to be indented.
**Remarks**
The default value is true. If the value is false, it will reduce the size of the xml file
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
### setExportColumnIndexOfCell(boolean value) {#setExportColumnIndexOfCell-boolean-}
```
public void setExportColumnIndexOfCell(boolean value)
```
The default value is false, it means that column index will be ignored if the cell is contiguous to the previous cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setIndentedFormatting(boolean value) {#setIndentedFormatting-boolean-}
```
public void setIndentedFormatting(boolean value)
```
Causes child elements to be indented.
**Remarks**
The default value is true. If the value is false, it will reduce the size of the xml file
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setLimitAsXls(boolean value) {#setLimitAsXls-boolean-}
```
public void setLimitAsXls(boolean value)
```
Limit as xls, the max row index is 65535 and the max column index is 255.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```
Indicates whether refreshing chart cache data
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
