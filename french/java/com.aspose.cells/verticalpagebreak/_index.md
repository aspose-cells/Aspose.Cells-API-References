---
title: "VerticalPageBreak"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente un saut de page vertical."
type: docs
url: /fr/java/com.aspose.cells/verticalpagebreak/
---

**Inheritance:**
java.lang.Object
```
public class VerticalPageBreak
```

Encapsule l'objet qui représente un saut de page vertical.

**Example**

```
         Workbook excel = new Workbook();
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtient l'index de colonne du saut de page vertical. |
| [getEndRow()](#getEndRow--) | Obtient l'index de ligne de fin du saut de page vertical. |
| [getStartRow()](#getStartRow--) | Obtient l'index de ligne de début du saut de page vertical. |
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
| Paramètre | Type | Description |
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


Obtient l'index de colonne du saut de page vertical.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Obtient l'index de ligne de fin du saut de page vertical.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Obtient l'index de ligne de début du saut de page vertical.

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

