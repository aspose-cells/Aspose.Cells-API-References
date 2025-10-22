##SplitPartInfo
Represents the information of one input/output for multiple inputs/outputs such as current page to be rendered when converting spreadsheet to image.
**Inheritance:**
java.lang.Object
```
public class SplitPartInfo
```
Represents the information of one input/output for multiple inputs/outputs, such as current page to be rendered when converting spreadsheet to image.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPartIndex()](#getPartIndex--) | Index of current part in sequence(0 based) |
| [getSheetIndex()](#getSheetIndex--) | Index of the sheet where current part is in. -1 denotes there is only one sheet. |
| [getSheetName()](#getSheetName--) | Name of the sheet where current part is in. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getPartIndex() {#getPartIndex--}
```
public int getPartIndex()
```
Index of current part in sequence(0 based). -1 means there are no multiple parts so the result is single.
**Remarks**
If multiple sheets need to be processed and every sheet is processed(split) separately, the part index always starts from 0 for every sheet. For example, when converting workbook to images, it represents the output page index of currently processed sheet. And -1 denotes there is only one page for current sheet.
**Returns:**
int
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```
Index of the sheet where current part is in. -1 denotes there is only one sheet.
**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```
Name of the sheet where current part is in.
**Remarks**
May be null for some situations, such as when rendering the whole workbook to tiff image.
**Returns:**
java.lang.String
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
