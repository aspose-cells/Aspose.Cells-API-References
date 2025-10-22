##PdfBookmarkEntry
PdfBookmarkEntry is an entry in pdf bookmark.
**Inheritance:**
java.lang.Object
```
public class PdfBookmarkEntry
```
PdfBookmarkEntry is an entry in pdf bookmark. if Text property of current instance is null or "", current instance will be hidden and children will be inserted on current level.
**Example**
```
Workbook workbook = new Workbook();
workbook.getWorksheets().add();
workbook.getWorksheets().add();
Cell cellInPage1 = workbook.getWorksheets().get(0).getCells().get("A1");
Cell cellInPage2 = workbook.getWorksheets().get(1).getCells().get("A1");
Cell cellInPage3 = workbook.getWorksheets().get(2).getCells().get("A1");
cellInPage1.putValue("page1");
cellInPage2.putValue("page2");
cellInPage3.putValue("page3");
PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry();
pbeRoot.setText("root");  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
pbeRoot.setDestination(cellInPage1);
pbeRoot.setSubEntry(new ArrayList());
pbeRoot.setOpen(false);
PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry();
subPbe1.setText("section1");
subPbe1.setDestination(cellInPage2);
PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry();
subPbe2.setText("section2");
subPbe2.setDestination(cellInPage3);
pbeRoot.getSubEntry().add(subPbe1);
pbeRoot.getSubEntry().add(subPbe2);
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.setBookmark(pbeRoot);
workbook.save("output_bookmark.pdf", saveOptions);
```
## Constructors
| Constructor | Description |
| --- | --- |
| [PdfBookmarkEntry()](#PdfBookmarkEntry--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestination()](#getDestination--) | The cell to which the bookmark link. |
| [getDestinationName()](#getDestinationName--) | Gets name of destination. |
| [getSubEntry()](#getSubEntry--) | SubEntry of a bookmark. |
| [getText()](#getText--) | Title of a bookmark. |
| [hashCode()](#hashCode--) |  |
| [isCollapse()](#isCollapse--) | When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
| [isOpen()](#isOpen--) | When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapse(boolean value)](#setCollapse-boolean-) | When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
| [setDestination(Cell value)](#setDestination-com.aspose.cells.Cell-) | The cell to which the bookmark link. |
| [setDestinationName(String value)](#setDestinationName-java.lang.String-) | Sets name of destination. |
| [setOpen(boolean value)](#setOpen-boolean-) | When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| [setSubEntry(ArrayList value)](#setSubEntry-java.util.ArrayList-) | SubEntry of a bookmark. |
| [setText(String value)](#setText-java.lang.String-) | Title of a bookmark. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfBookmarkEntry() {#PdfBookmarkEntry--}
```
public PdfBookmarkEntry()
```
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
### getDestination() {#getDestination--}
```
public Cell getDestination()
```
The cell to which the bookmark link.
**Returns:**
[Cell](../../com.aspose.cells/cell)
### getDestinationName() {#getDestinationName--}
```
public String getDestinationName()
```
Gets name of destination.
**Remarks**
If destination name is set, the destination will be defined as a named destination with this name.
**Returns:**
java.lang.String
### getSubEntry() {#getSubEntry--}
```
public ArrayList getSubEntry()
```
SubEntry of a bookmark.
**Returns:**
java.util.ArrayList
### getText() {#getText--}
```
public String getText()
```
Title of a bookmark.
**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isCollapse() {#isCollapse--}
```
public boolean isCollapse()
```
When this property is true, the bookmarkentry will collapse, otherwise it will expand.
**Returns:**
boolean
### isOpen() {#isOpen--}
```
public boolean isOpen()
```
When this property is true, the bookmarkentry will expand, otherwise it will collapse.
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
### setCollapse(boolean value) {#setCollapse-boolean-}
```
public void setCollapse(boolean value)
```
When this property is true, the bookmarkentry will collapse, otherwise it will expand.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setDestination(Cell value) {#setDestination-com.aspose.cells.Cell-}
```
public void setDestination(Cell value)
```
The cell to which the bookmark link.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Cell](../../com.aspose.cells/cell) |  |
### setDestinationName(String value) {#setDestinationName-java.lang.String-}
```
public void setDestinationName(String value)
```
Sets name of destination.
**Remarks**
If destination name is set, the destination will be defined as a named destination with this name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOpen(boolean value) {#setOpen-boolean-}
```
public void setOpen(boolean value)
```
When this property is true, the bookmarkentry will expand, otherwise it will collapse.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSubEntry(ArrayList value) {#setSubEntry-java.util.ArrayList-}
```
public void setSubEntry(ArrayList value)
```
SubEntry of a bookmark.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.ArrayList |  |
### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```
Title of a bookmark.
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
