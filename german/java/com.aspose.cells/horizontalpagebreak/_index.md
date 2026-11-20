---
title: "HorizontalPageBreak"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das einen horizontalen Seitenumbruch darstellt."
type: docs
url: /de/java/com.aspose.cells/horizontalpagebreak/
---

**Inheritance:**
java.lang.Object
```
public class HorizontalPageBreak
```

Kapselt das Objekt, das einen horizontalen Seitenumbruch darstellt.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Add a page break at cell Y30
         int Index = worksheet.getHorizontalPageBreaks().add("Y30");
 
         //get the newly added horizontal page break
         HorizontalPageBreak hPageBreak = worksheet.getHorizontalPageBreaks().get(Index);
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | Gibt den Endspaltenindex dieses horizontalen Seitenumbruchs zurück. |
| [getRow()](#getRow--) | Gibt den nullbasierten Zeilenindex zurück. |
| [getStartColumn()](#getStartColumn--) | Gibt den Startspaltenindex dieses horizontalen Seitenumbruchs zurück. |
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
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Gibt den Endspaltenindex dieses horizontalen Seitenumbruchs zurück.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


Gibt den nullbasierten Zeilenindex zurück.

**Returns:**
int
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Gibt den Startspaltenindex dieses horizontalen Seitenumbruchs zurück.

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

