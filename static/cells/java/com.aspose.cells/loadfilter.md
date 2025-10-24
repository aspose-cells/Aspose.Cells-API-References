##LoadFilter
Represents the filter that provides options for loading data when loading workbook from template.
**Inheritance:**
java.lang.Object
```
public class LoadFilter
```
Represents the filter that provides options for loading data when loading workbook from template.
**Remarks**
User may specify the filter options or implement their own LoadFilter to specify how to load data.
**Example**
The following example shows how to determine the filter options according to worksheet's properties.
```
class LoadFilterSheet extends LoadFilter
{
public /*override*/ void startSheet(Worksheet sheet)
{
if ("Sheet1".equals(sheet.getName()))
{
setLoadDataFilterOptions(LoadDataFilterOptions.ALL);
}
else
{
setLoadDataFilterOptions(LoadDataFilterOptions.STRUCTURE);
}
}
}
LoadOptions opts = new LoadOptions();
opts.setLoadFilter(new LoadFilterSheet());
Workbook wb = new Workbook("template.xlsx", opts);
//Custom LoadFilter implementation
```
## Constructors
| Constructor | Description |
| --- | --- |
| [LoadFilter()](#LoadFilter--) | Constructs one LoadFilter with default filter options LoadDataFilterOptions.All. |
| [LoadFilter(int opts)](#LoadFilter-int-) | Constructs one LoadFilter with given filter options. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLoadDataFilterOptions()](#getLoadDataFilterOptions--) | The filter options to denote what data should be loaded. |
| [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--) | Specifies the sheets(indices) and order to be loaded. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLoadDataFilterOptions(int value)](#setLoadDataFilterOptions-int-) | The filter options to denote what data should be loaded. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Prepares filter options before loading given worksheet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LoadFilter() {#LoadFilter--}
```
public LoadFilter()
```
Constructs one LoadFilter with default filter options LoadDataFilterOptions.All.
### LoadFilter(int opts) {#LoadFilter-int-}
```
public LoadFilter(int opts)
```
Constructs one LoadFilter with given filter options.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | int | [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions). the default filter options |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getLoadDataFilterOptions() {#getLoadDataFilterOptions--}
```
public int getLoadDataFilterOptions()
```
The filter options to denote what data should be loaded.
See [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).
**Returns:**
int
### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}
```
public int[] getSheetsInLoadingOrder()
```
Specifies the sheets(indices) and order to be loaded. Default is null, that denotes to load all sheets in the default order in template file. If not null and some sheet's index is not in the returned array, then the sheet will not be loaded.
**Returns:**
int[]
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
### setLoadDataFilterOptions(int value) {#setLoadDataFilterOptions-int-}
```
public void setLoadDataFilterOptions(int value)
```
The filter options to denote what data should be loaded.
See [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public void startSheet(Worksheet sheet)
```
Prepares filter options before loading given worksheet. User's implementation of LoadFilter can change the LoadDataFilterOptions here to denote how to load data for this worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | The worksheet to be loaded. There are only few properties can be used for the given worksheet object here because most data and properties have not been loaded. The available properties are: Name, Index, VisibilityType |
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
