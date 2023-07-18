---
title: SheetSet
second_title: Aspose.Cells for Java API Reference
description: Describes a set of sheets.
type: docs
url: /java/com.aspose.cells/sheetset/
---

**Inheritance:**
java.lang.Object
```
public class SheetSet
```

Describes a set of sheets.
## Constructors

| Constructor | Description |
| --- | --- |
| [SheetSet(int[] sheets)](#SheetSet-int---) | Creates a sheet set based on exact sheet indexes. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActive()](#getActive--) | Gets a set with active sheet of the workbook. |
| [getAll()](#getAll--) | Gets a set with all sheets of the workbook in their original order. |
| [getClass()](#getClass--) |  |
| [getVisible()](#getVisible--) | Gets a set with visible sheets of the workbook in their original order. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetSet(int[] sheets) {#SheetSet-int---}
```
public SheetSet(int[] sheets)
```


Creates a sheet set based on exact sheet indexes.

**Remarks**

If a sheet is encountered that is not in the workbook, an exception will be thrown during rendering.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheets | int[] | zero based sheet indexes. |

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
### getActive() {#getActive--}
```
public static SheetSet getActive()
```


Gets a set with active sheet of the workbook.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getAll() {#getAll--}
```
public static SheetSet getAll()
```


Gets a set with all sheets of the workbook in their original order.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getVisible() {#getVisible--}
```
public static SheetSet getVisible()
```


Gets a set with visible sheets of the workbook in their original order.

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
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

