##ExternalLinkCollection
Represents external links collection in a workbook.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
java.lang.Iterable
```
public class ExternalLinkCollection implements Iterable
```
Represents external links collection in a workbook.
**Example**
```
//Open a file with external links
Workbook workbook = new Workbook("book1.xls");
//Change external link data source
workbook.getWorksheets().getExternalLinks().get(0).setDataSource("d:\\link.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [add(int directoryType, String fileName, String[] sheetNames)](#add-int-java.lang.String-java.lang.String---) | Add an external link . |
| [add(String fileName, String[] sheetNames)](#add-java.lang.String-java.lang.String---) | Adds an external link. |
| [clear()](#clear--) | Removes all external links. |
| [clear(boolean updateReferencesAsLocal)](#clear-boolean-) | Removes all external links. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [ExternalLink](../../com.aspose.cells/externallink) element at the specified index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the number of elements actually contained in the collection. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Get an enumerator that iterates through this collection. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Removes the specified external link from the workbook. |
| [removeAt(int index, boolean updateReferencesAsLocal)](#removeAt-int-boolean-) | Removes the specified external link from the workbook. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int directoryType, String fileName, String[] sheetNames) {#add-int-java.lang.String-java.lang.String---}
```
public int add(int directoryType, String fileName, String[] sheetNames)
```
Add an external link .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directoryType | int | [DirectoryType](../../com.aspose.cells/directorytype). The directory type of the file name. |
| fileName | java.lang.String | the file name. |
| sheetNames | java.lang.String[] | All sheet names of the external file. |
**Returns:**
int - The position of the external name in this list.
### add(String fileName, String[] sheetNames) {#add-java.lang.String-java.lang.String---}
```
public int add(String fileName, String[] sheetNames)
```
Adds an external link.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The external file name. |
| sheetNames | java.lang.String[] | All sheet names of the external file. |
**Returns:**
int - The position of the external name in this list.
### clear() {#clear--}
```
public void clear()
```
Removes all external links.
**Remarks**
When removing external links, all formulas that reference to them will be removed too because the references become invalid.
### clear(boolean updateReferencesAsLocal) {#clear-boolean-}
```
public void clear(boolean updateReferencesAsLocal)
```
Removes all external links.
**Remarks**
If references are required to be updated, those references of external links in formulas will be changed to current workbook when it is possible. For example, one cell's original formula is "='externalsource.xlam'!customfunction()", after removing external links, the formula will become "=customfunction()"; When the original formula is "='[externalsource.xlam]Sheet1'!$A$1", according to whether there is one sheet with name "Sheet1" in current workbook: if true, the formula will become "=Sheet1!$A$1"; if false, the formula will become "=\#REF!$A$1".
If references are not required to be updated, all formulas with references to external links will be removed too because those references become invalid.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Whether update all references of external links in formulas to references of current workbook itself. |
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
### get(int index) {#get-int-}
```
public ExternalLink get(int index)
```
Gets the [ExternalLink](../../com.aspose.cells/externallink) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[ExternalLink](../../com.aspose.cells/externallink) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```
Gets the number of elements actually contained in the collection.
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```
Get an enumerator that iterates through this collection.
**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Removes the specified external link from the workbook.
**Remarks**
When removing the external link, all formulas that reference to it will be removed too because the references become invalid.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the external link to be removed. |
### removeAt(int index, boolean updateReferencesAsLocal) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean updateReferencesAsLocal)
```
Removes the specified external link from the workbook.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the external link to be removed. |
| updateReferencesAsLocal | boolean | Whether update all references of given external link to reference of current workbook itself. Check [clear(boolean)](../../com.aspose.cells/externallinkcollection\#clear-boolean-) to get more details about this parameter. |
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
