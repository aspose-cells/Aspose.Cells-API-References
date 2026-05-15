---
title: HyperlinkLoadMode
second_title: Aspose.Cells for Java API Reference
description: Specifies how hyperlinks are handled when loading HTML.
type: docs
url: /java/com.aspose.cells/hyperlinkloadmode/
---

**Inheritance:**
java.lang.Object
```
public final class HyperlinkLoadMode
```

Specifies how hyperlinks are handled when loading HTML.
## Fields

| Field | Description |
| --- | --- |
| [ALLOW_MULTIPLE](#ALLOW-MULTIPLE) | All hyperlinks in a cell are added to [Worksheet.getHyperlinks()](../../com.aspose.cells/worksheet\#getHyperlinks--). |
| [NORMAL](#NORMAL) | Only the first hyperlink in a cell is loaded, subsequent ones are ignored. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ALLOW_MULTIPLE {#ALLOW-MULTIPLE}
```
public static final int ALLOW_MULTIPLE
```


All hyperlinks in a cell are added to [Worksheet.getHyperlinks()](../../com.aspose.cells/worksheet\#getHyperlinks--). Note that MS Excel itself supports only one hyperlink per cell, so this option may produce files that Excel cannot fully render.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Only the first hyperlink in a cell is loaded, subsequent ones are ignored.

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

