---
title: "VerticalPageBreak"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das einen vertikalen Seitenumbruch darstellt."
type: docs
url: /de/java/com.aspose.cells/verticalpagebreak/
---

**Inheritance:**
java.lang.Object
```
public class VerticalPageBreak
```

Kapselt das Objekt, das einen vertikalen Seitenumbruch darstellt.

**Example**

```
         Workbook excel = new Workbook();
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Ruft den Spaltenindex des vertikalen Seitenumbruchs ab. |
| [getEndRow()](#getEndRow--) | Ruft den Endzeilenindex des vertikalen Seitenumbruchs ab. |
| [getStartRow()](#getStartRow--) | Ruft den Startzeilenindex des vertikalen Seitenumbruchs ab. |
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
| Parameter | Typ | Beschreibung |
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
### getColumn() {#getColumn--}
```
public int getColumn()
```


Ruft den Spaltenindex des vertikalen Seitenumbruchs ab.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Ruft den Endzeilenindex des vertikalen Seitenumbruchs ab.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Ruft den Startzeilenindex des vertikalen Seitenumbruchs ab.

**Returns:**
int
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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

