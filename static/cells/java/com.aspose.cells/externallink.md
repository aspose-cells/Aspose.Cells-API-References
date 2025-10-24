##ExternalLink
Represents an external link in a workbook.
**Inheritance:**
java.lang.Object
```
public class ExternalLink
```
Represents an external link in a workbook.
**Example**
```
//Open a file with external links
Workbook workbook = new Workbook("book1.xls");
//Get External Link
ExternalLink externalLink = workbook.getWorksheets().getExternalLinks().get(0);
//Change External Link's Data Source
externalLink.setDataSource("d:\\link.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [addExternalName(String text, String referTo)](#addExternalName-java.lang.String-java.lang.String-) | Adds an external name. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDataSource()](#getDataSource--) | Represents data source of the external link. |
| [getOriginalDataSource()](#getOriginalDataSource--) | Represents stored data source of the external link. |
| [getPathType()](#getPathType--) | Get the path type of this external link |
| [getType()](#getType--) | Gets the type of external link. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Indicates whether this external link is referenced by others. |
| [isVisible()](#isVisible--) | Indicates whether this external link is visible in MS Excel. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDataSource(String value)](#setDataSource-java.lang.String-) | Represents data source of the external link. |
| [setOriginalDataSource(String value)](#setOriginalDataSource-java.lang.String-) | Represents stored data source of the external link. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addExternalName(String text, String referTo) {#addExternalName-java.lang.String-java.lang.String-}
```
public void addExternalName(String text, String referTo)
```
Adds an external name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| text | java.lang.String | The text of the external name. If the external name belongs to a worksheet, the text should be as Sheet1!Text. |
| referTo | java.lang.String | The referTo of the external name. It must be a cell or the range. |
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
### getDataSource() {#getDataSource--}
```
public String getDataSource()
```
Represents data source of the external link.
**Returns:**
java.lang.String
### getOriginalDataSource() {#getOriginalDataSource--}
```
public String getOriginalDataSource()
```
Represents stored data source of the external link.
**Returns:**
java.lang.String
### getPathType() {#getPathType--}
```
public String getPathType()
```
Get the path type of this external link
**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```
Gets the type of external link.
See [ExternalLinkType](../../com.aspose.cells/externallinktype).
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```
Indicates whether this external link is referenced by others.
**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```
Indicates whether this external link is visible in MS Excel.
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
### setDataSource(String value) {#setDataSource-java.lang.String-}
```
public void setDataSource(String value)
```
Represents data source of the external link.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOriginalDataSource(String value) {#setOriginalDataSource-java.lang.String-}
```
public void setOriginalDataSource(String value)
```
Represents stored data source of the external link.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
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
